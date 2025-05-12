# Rangebound Algorithm

This repository contains an implementation of a range compression algorithm for financial markets, designed to identify periods of market consolidation and potential breakouts.

## Overview

The Rangebound Algorithm analyzes historical price data to identify periods where an asset is trading within a confined range. The algorithm calculates compression metrics using various methods, including:

1. A volatility-based expected range using historical volatility
2. A historical high-low range comparison over different time periods
3. Compression scores that indicate when prices are likely to break out of established ranges

## Requirements

This project requires Python 3.7+ and several dependencies, which are listed in the `requirements.txt` file. To set up the virtual environment and install the dependencies, follow the installation instructions below.

## Installation

1. Clone the repository:
```
git clone https://github.com/yourusername/RangeboundAlgorithm.git
cd RangeboundAlgorithm
```

2. Create a virtual environment:
```
python -m venv venv
```

3. Activate the virtual environment:

   On Windows:
   ```
   venv\Scripts\activate
   ```

   On macOS/Linux:
   ```
   source venv/bin/activate
   ```

4. Install the required packages:
```
pip install -r requirements.txt
```

## Usage

The primary implementation is in the Jupyter notebook `RangeboundPython.ipynb`. You can run the notebook using Jupyter:

```
jupyter notebook RangeboundPython.ipynb
```

The notebook demonstrates:
- Loading and preprocessing financial data
- Calculating volatility and range metrics
- Computing compression scores
- Visualizing the results

## Algorithm Parameters

The algorithm uses several configurable parameters:

- `vol_window`: Window size for volatility calculation (default: 1095 days, roughly 3 years)
- `range_window`: Window size for current range calculation (default: 60 days, roughly 2 months)
- `z_score`: Z-score for the expected range calculation (default: 1.5)

These parameters can be adjusted based on the specific asset class or timeframe being analyzed.

## Features

- **Volatility-Based Compression Scores**: Calculate compression based on historical volatility
- **Historical Range Compression**: Calculate compression based on multi-year high-low ranges
- **Visualization Tools**: Plot compression scores along with price to identify potential breakout points
- **Multiple Time Frame Analysis**: Supports analysis across different time frames

## License

[Specify the license here]

## Contact

[Your contact information] 