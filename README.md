# 📊 Fear & Greed Index vs Trader Behavior

## Overview
This project explores how market sentiment — measured by the Fear & Greed Index — influences individual trading behavior. By merging sentiment data with real trade logs, we uncover how emotional market conditions affect leverage, direction, and profitability.

## Data Sources
- **Trader Data**: Timestamped trades with execution price, size, direction, and PnL.
- **Fear & Greed Index**: Extracted from a malformed PDF and cleaned into structured CSV with daily sentiment scores and classifications.

## Key Steps
1. **PDF Extraction**: Used `pdfplumber` to extract tabular sentiment data from a misnamed `.csv` file.
2. **Data Cleaning**: Normalized timestamps, handled encoding issues, and filtered invalid rows.
3. **Merging**: Joined sentiment and trader data on calendar date.
4. **Visualization**: Created time series and box plots to explore sentiment impact on PnL and leverage.

## Insights
- 📈 **Greed Days**: Traders showed higher leverage but mixed profitability.
- 📉 **Fear Days**: Lower trade volume, but more conservative and often more profitable trades.
- 📊 **Sentiment Score Trends**: Clear cyclical patterns that align with market volatility.

## Tools Used
- Python: `pandas`, `matplotlib`, `seaborn`, `pdfplumber`
- Google Colab for cloud-based analysis and visualization


## 🔗 Project Access
You can view and download the full project folder [here](YOUR_GOOGLE_DRIVE_OR_GITHUB_LINK).

## Next Steps
- Add rolling averages and volatility overlays
- Explore predictive modeling using sentiment as a feature
- Package into a dashboard or interactive web app


