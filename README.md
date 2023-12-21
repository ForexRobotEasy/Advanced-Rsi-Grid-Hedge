# Advanced RSI Grid Hedge Expert Advisor

This expert advisor implements a trading algorithm based on RSI indicators, grid hedging system, and trend filter. It does not employ martingale techniques. The recommended sets with specific parameters and currency pairs are SetH1_v1 and SetH1_v2.

## Input Variables
- RSI_Period1 (int): RSI period for the first RSI indicator.
- RSI_Period2 (int): RSI period for the second RSI indicator.
- Grid_Size (double): Grid size in pips.
- Lot_Size (double): Initial lot size.
- Max_Lots (double): Maximum allowed lot size.
- Stop_Loss (double): Stop loss in pips.
- Take_Profit (double): Take profit in pips.
- Trend_Filter_Period (double): Period for the trend filter.

## Recommended Currency Pairs
- SetH1_v1: AUDUSD, EURCAD, GBPCAD, EURJPY, EURNZD, CHFJPY, NZDUSD.
- SetH1_v2: AUDCHF.

## Trading Logic
The expert advisor uses a combination of RSI indicators, grid hedging, and trend filter to identify high-probability market reversals. It checks for buy and sell signals based on the RSI values and the trend filter.

### Buy Signal
A buy signal is generated if both RSI values are below 30.

### Sell Signal
A sell signal is generated if both RSI values are above 70.

### Trend Filter Signal
A trend filter signal is generated if the current close price is above the moving average.

## Placing Trades
If the recommended set, buy signal, and trend filter signal are all present, a buy order is placed with the specified lot size, stop loss, and take profit. If the recommended set, sell signal, and trend filter signal are all present, a sell order is placed with the specified parameters.

## Additional Information
Forex Robot Easy is not the official developer of this product. We only provide a sample code that can work as described in this product. For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Advanced RSI Grid Hedge Expert Advisor](https://forexroboteasy.com/forex-robot-review/review-advanced-rsi-grid-hedge-expert-advisor-for-high-probability-market-reversals/). To find the official developer of this product, please refer to MQL5.
