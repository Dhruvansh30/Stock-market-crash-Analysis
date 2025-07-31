# Stock Market Crash Analysis

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Plotly](https://img.shields.io/badge/Plotly-%233F4F75.svg?style=for-the-badge&logo=plotly&logoColor=white)

A comprehensive analysis of stock market crashes using historical Sensex data, identifying crash periods through drawdown analysis and visualizing market behavior during turbulent periods.

## Features

- **Crash Detection**: Identifies market crashes using drawdown thresholds
- **Cluster Analysis**: Groups consecutive crash days into significant events
- **Interactive Visualizations**: 
  - Price trends during crash periods
  - Daily returns analysis
  - Drawdown evolution visualization
- **Statistical Analysis**: Measures duration and severity of market downturns

## Methodology

1. **Data Preparation**:
   - Loads historical Sensex data (Open, High, Low, Close, Volume)
   - Calculates daily returns and cumulative maximums

2. **Crash Identification**:
   - Computes drawdown percentages
   - Flags crash days based on user-defined thresholds

3. **Cluster Analysis**:
   - Groups nearby crash days into significant events
   - Calculates cluster duration and severity

4. **Visualization**:
   - Interactive Plotly charts showing:
     - Price trends with crash periods highlighted
     - Return distributions during crashes
     - Drawdown progression

## Installation

```bash
git clone https://github.com/Dhruvansh30/Stock-market-crash-Analysis.git
cd Stock-market-crash-Analysis
pip install -r requirements.txt

Usage
Run the Jupyter notebook:

bash
jupyter notebook SMC.ipynb
Modify parameters in the "Configuration" section:

python
drawdown_threshold = -20  # Percentage threshold for crash detection
crash_threshold_daily = -3  # Daily return threshold
Execute all cells to perform analysis and generate visualizations


Requirements
Python 3.8+

pandas

numpy

plotly

jupyter
