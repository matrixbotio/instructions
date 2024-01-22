# 🔎 Indicators

**Indicators** (filters) help the bot find the optimal entry point for each new round. With well-configured filters, the bot will open a position in such a way that it can quickly and profitably close it with a take profit order.

Entry indicators are configured on the bot editing page [https://matrixbot.io/edit/new](https://matrixbot.io/edit/new)

#### RSI

<div align="left">

<figure><img src=".gitbook/assets/image (12).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

RSI (Relative Strength Index) is a technical indicator that measures the speed and change of price movements. RSI oscillates between 0 and 100 and is typically used to determine overbought or oversold conditions in the market.

RSI is calculated based on average gains and losses over a specific period of time, usually a 14-day period. When RSI rises above 70, it may indicate that the asset is overbought, presenting a selling opportunity. Similarly, when RSI falls below 30, it may indicate oversold conditions, providing a potential buying opportunity.

#### CCI

CCI (Commodity Channel Index) is another popular technical indicator that measures the current price position relative to the average price level over a specific period of time. This indicator can help traders identify when an asset starts deviating from its "normal" price range.

CCI is calculated by subtracting the average asset price from its current price and then dividing the result by the average absolute deviation of the average price. A 20-day period is commonly used. CCI fluctuates in a wider range than RSI, and its values can significantly exceed 100 or drop below -100.

When CCI is above +100, it may indicate overbought market conditions, suggesting that the price may soon start to correct downwards. When the indicator drops below -100, it may signal oversold conditions, which could foreshadow an upward correction.

Just like with RSI, it is important to use CCI in combination with other indicators and methods of technical analysis. This helps reduce the risk of false signals and increases the likelihood of successful trading. CCI settings, including the chosen period, can be adapted to match specific trading strategies and market conditions.

#### MA

<div align="left">

<figure><img src=".gitbook/assets/image (13).png" alt="" width="289"><figcaption></figcaption></figure>

</div>

MA (Moving Average) is one of the most basic and widely used technical indicators in financial market analysis. Moving averages help smooth price data to create a visible trend line that shows the overall market direction. This makes it particularly useful for identifying overall price trends and potential reversal points.

Here, a simple moving average (SMA) is used, calculated by summing the closing prices of the asset over a certain number of time periods (e.g., days) and then dividing this sum by the number of periods.

When a shorter moving average (e.g., 10-day MA) crosses below a longer moving average (e.g., 50-day MA) from above, it may signal a potential sell (bearish cross). If the shorter moving average crosses above the longer one from below, it may be a signal to buy (bullish cross).

Moving averages can also be used to determine support and resistance levels. For example, in an uptrend, the longer moving average often serves as a support level, while in a downtrend, it may act as a resistance level.

#### Bollinger Bands

<div align="left">

<figure><img src=".gitbook/assets/image (14).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

Bollinger Bands are a technical indicator developed by John Bollinger in the 1980s. This indicator consists of a set of lines, usually three, that are placed on a price chart. The central line is a simple moving average (usually 20-day), while the other two lines represent standard deviations of the price from this moving average, typically at a distance of two standard deviations above and below.

Bollinger Bands are useful for determining market volatility. When the bands expand, it indicates increasing volatility, and when they contract, it indicates decreasing volatility. Additionally, they help identify overbought and oversold conditions of an asset.

In the context of automated trading, Bollinger Bands can be used to generate trading signals:

1. **Band Breakouts**: When the price closes above the upper band, it can be considered a buy signal. Similarly, closing below the lower band can be a sell signal.
2. **Bollinger Bounces**: Prices often bounce off the upper and lower bands. When the price touches one of the bands, traders may consider entering in the opposite direction.
3. **Band Squeezes**: Narrow bands indicate low volatility and may foreshadow a future strong momentum move. Trading strategies can utilize this state to anticipate breakouts.

#### ADX

<div align="left">

<figure><img src=".gitbook/assets/image (15).png" alt="" width="320"><figcaption></figcaption></figure>

</div>

ADX (Average Directional Index) is a technical indicator developed by J. Welles Wilder that helps measure the strength and direction of a trend. ADX ranges from 0 to 100, where higher values indicate a stronger trend regardless of its direction. The ADX line shows the strength of the trend. Values above 25 usually indicate a strong trend, while values below 20 may indicate a weak or absent trend.

#### ATR

<div align="left">

<figure><img src=".gitbook/assets/image (16).png" alt="" width="375"><figcaption></figcaption></figure>

</div>

ATR (Average True Range) is another technical indicator developed by J. Welles Wilder. It is designed to measure market volatility without considering the direction of price movement. ATR is calculated based on the "true range" of an asset, which takes into account the current price range (the difference between the highest and lowest prices), as well as the difference between the current highest and lowest prices and the previous closing price.

The Average True Range is typically calculated over a 14-day period, although the period can be adjusted depending on the trading strategy. ATR does not indicate the direction of price movement; it simply measures the level of volatility. Higher ATR values indicate higher volatility, while lower values indicate lower volatility.

#### VOLUME

The volume indicator is used to analyze the trading volume in the selected pair. Volume is considered an important tool as it can help determine the strength or weakness of a trend.

The volume indicator typically returns a numerical value representing the trading volume for each period (e.g., day or hour) in the selected instrument.

#### OPEN, CLOSE, HIGH, LOW

OPEN, CLOSE, HIGH, and LOW levels are key elements of price chart analysis and can be used as indicators or in combination with other indicators.

1. HIGH and LOW levels can indicate areas of resistance and support.
   * **Trends**: CLOSE levels can be used to determine the overall trend. For example, a sequence of increasing CLOSE levels indicates an uptrend.
   * **Reversals**: Candlestick patterns such as a hammer or a doji star use these levels to identify potential reversal points.
2. In combination with other indicators:
   * **Moving Average (MA) crossovers**: Price level crossovers with moving averages can signal a potential trend change.
   * **In conjunction with volume indicators**: Trading volume at HIGH and LOW levels can confirm the strength or weakness of a trend.
   * **Convergence/divergence with indicators like RSI or MACD**: Differences between price behavior (e.g., new highs or lows) and indicator readings can indicate potential convergence or divergence, which can be a signal for a trend change.
