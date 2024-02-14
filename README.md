# Forex Robot Easy Team - Support Resistance Propulsion Targets MT5

This code is designed to draw support and resistance lines based on historical data and identify propulsion candle gaps on the chart. It serves as a tool for optimizing forex trades.

## How it Works

The code consists of two main functions: `DrawSupportResistanceLines()` and `IdentifyPropulsionCandleGaps()`. These functions are called in the `OnStart()` function, which serves as the entry point of the program.

### DrawSupportResistanceLines()

This function is responsible for drawing support and resistance lines using historical data. It identifies the last two days, six weeks, and six months data and creates objects to represent the lines.

- `lastTwoDays` variable stores the datetime value of the last two days.
- `lastSixWeeks` variable stores the datetime value of the last six weeks.
- `lastSixMonths` variable stores the datetime value of the last six months.

Support Lines:
- `ObjectCreate()` function is used to create support lines with different styles and colors at specific price levels.
- `ObjectSetInteger()` function is used to set the color and style properties for each support line.

Resistance Lines:
- Similar to support lines, resistance lines are created using the `ObjectCreate()` function.
- `ObjectSetInteger()` function is used to set the color and style properties for each resistance line.

### IdentifyPropulsionCandleGaps()

This function loops through all candles and calculates the gap between the current candle and the next candle. If the gap is significant (greater than 0.01), it highlights the gap on the chart.

- A for loop is used to iterate through all the candles.
- The `MathAbs()` function calculates the absolute difference between the close and open prices of the candles.
- If the gap is significant, a rectangle label object is created using the `ObjectCreate()` function to highlight the gap on the chart.
- `ObjectSetInteger()` function is used to set the color and style properties for each propulsion gap.
- `ObjectSetText()` function is used to set the text properties for the propulsion gap label.

## Product Description

Support Resistance Propulsion Targets MT5 is a powerful tool designed to optimize forex trades by drawing support and resistance lines and identifying propulsion candle gaps on the chart. It is a valuable asset for traders looking to make informed trading decisions based on historical data.

With Support Resistance Propulsion Targets MT5, traders can easily visualize and analyze support and resistance levels based on the last two days, six weeks, and six months data. This provides valuable insights into potential price reversal or breakout points.

Additionally, the tool identifies significant propulsion candle gaps, highlighting them on the chart. These gaps indicate strong momentum and potential trading opportunities.

Please note that ForexRobotEasy is not the official developer of this product. We provide this sample code to demonstrate how the product works. For detailed reviews and trading results of Support Resistance Propulsion Targets MT5, please visit the official developer's website [here](https://forexroboteasy.com/forex-robot-review/review-support-resistance-propulsion-targets-mt5-optimizing-forex-trades/). To access the official developer, please use MQL5.
