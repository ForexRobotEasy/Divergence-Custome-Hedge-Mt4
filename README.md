# Divergence Custome Hedge Mt4

Divergence Custome Hedge Mt4 is an expert advisor (EA) for MetaTrader 4 that uses the MACD indicator to identify buy and sell signals in the market. This EA is developed by the Forex Robot Easy Team and is available for download on their website forexroboteasy.com.

To use this EA, you need to include the necessary libraries: Trade.mqh and MACD.mqh. These libraries provide the functions and classes required for trading and calculating the MACD indicator.

The EA defines some constants to be used throughout the code. LOT_SIZE is set to 0.01, SLIPPAGE is set to 3, and MAX_LOSS_PIPS is set to 10. These constants can be adjusted according to your trading preferences.

The global variables trade and macd are initialized. trade is an instance of the CTrade class, which provides functions for trading operations, and macd is an instance of the CMACD class, which provides functions for calculating the MACD indicator.

The OnInit() function is called when the EA is initialized. In this function, the MACD indicator is initialized with the current symbol, the H1 timeframe, and the parameters 12, 26, and 9. The PRICE_CLOSE parameter is used to calculate the MACD indicator.

The OnDeinit() function is called when the EA is deinitialized. In this function, the resources used by the MACD indicator are cleaned up.

The OnTick() function is called on each tick of the market. In this function, the EA checks for buy and sell signals using the MACD indicator. If a buy signal is detected, a buy order is opened with the specified lot size, symbol, ask price, and slippage. If a sell signal is detected, a sell order is opened with the specified lot size, symbol, bid price, and slippage.

The EA also checks for open positions. If there are any open positions, the EA checks if the market has moved against the trade. If the market has moved against a buy position by more than MAX_LOSS_PIPS, a sell order is opened to hedge the position. If the market has moved against a sell position by more than MAX_LOSS_PIPS, a buy order is opened to hedge the position.

Please note that ForexRobotEasy is not the official developer of this product. We are only providing a sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/review-divergence-custome-hedge-mt4-improve-your-hedging-style-with-macd-signals/).
