# HFX61 Expert Advisor ReadMe

This ReadMe file provides an overview of the HFX61 Expert Advisor and describes its functionality, parameters, and usage.

## Description

The HFX61 Expert Advisor is designed for early trend detection in the Forex market. It scans all potential early trends across all timeframes, with a focus on the M15 timeframe. It predicts the direction of the market price using built-in indicators and oscillators. In case of a failed early trend, it incorporates a flat lot hedge with controlled order distance for risk management. It also includes an AUTO Trade Setting feature to automatically open positions.

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that can work as described in this product. To find the official developer of this product, please use MQL5.

## Developer

The HFX61 Expert Advisor is developed by the Forex Robot Easy Team. For more information about the developer and their other products, please visit their website: [Forex Robot Easy](https://www.forexroboteasy.com)

## Expert Advisor Parameters

The HFX61 Expert Advisor includes the following parameters:

- `AutoTradeSetting` (bool): Enable/Disable AUTO Trade Setting

## Expert Advisor Initialization

The `OnInit()` function is responsible for initializing necessary variables and indicators. It sets the default position opening settings as specified in the product description.

## Expert Advisor Start Function

The `OnTick()` function is the main logic of the Expert Advisor. It performs early trend detection and opens positions based on the detected trend. If the `AutoTradeSetting` parameter is enabled, it calculates the lot size and order distance for risk management and opens a position with the calculated values. If no trend is detected, it performs a hedge position with a flat lot and controlled order distance.

## Helper Functions

The Expert Advisor includes the following helper functions:

- `CalculateLotSize()`: Calculates the lot size based on the risk management strategy.
- `CalculateOrderDistance()`: Calculates the order distance based on the risk management strategy.
- `OpenPosition(double lotSize, double orderDistance)`: Opens a position with the given lot size and order distance.
- `HedgePosition(double lotSize, double orderDistance)`: Hedges a position with the given lot size and order distance.

## Expert Advisor Deinitialization

The `OnDeinit(const int reason)` function is responsible for performing necessary cleanup and deinitialization tasks.

## Additional Information

For detailed reviews and trading results of this product, please visit [this link](https://forexroboteasy.com/forex-robot-review/hfx-6-1-starter-review-expert-advisor-for-early-trend-detection-in-forex/). Please note that ForexRobotEasy is not the official developer of this product. We only show sample code that can work as described in this product.

To find the official developer of this product, please use MQL5.

Last Updated: 2022/01/01
