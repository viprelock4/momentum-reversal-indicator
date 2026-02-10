# Momentum Reversal Indicator (MRI) - User Guide

## What is MRI?

The Momentum Reversal Indicator (MRI) is a time-based indicator that anticipates trend exhaustion and potential price reversals. It is based on the TD Sequential by Tom DeMark, with customizations including Extensions A/B/C, multi-timeframe display, and support/resistance levels.

**Credits:** Larry Williams, Tom DeMark, Tyler Jenks, Martin Armstrong & Kevin O'Dowd

---

## Setup Count (1-9)

The core of MRI is the 9-count setup phase.

**Sell Setup (MRI Top):**
- Red numbers 1-8 appear above candles when each candle's close is higher than the close 4 bars earlier
- 9 consecutive bars meeting this condition completes the setup
- A red **▼ arrow** appears at count 9 — this is the **MRI Top** signal
- Indicates the bullish trend may be exhausting

**Buy Setup (MRI Bottom):**
- Green numbers 1-8 appear below candles when each candle's close is lower than the close 4 bars earlier
- A green **▲ arrow** appears at count 9 — this is the **MRI Bottom** signal
- Indicates the bearish trend may be exhausting

**Important:** The count resets immediately if any candle fails the comparison (close vs close[4]).

---

## Consecutive Counts

When the MRI signal (arrow) shows a number greater than 1, it means the signal has fired multiple times consecutively in the same direction without a reversal. For example:

- **2** = Two consecutive MRI tops/bottoms
- **3** = Three consecutive signals

Higher consecutive counts indicate a stronger trend that has repeatedly failed to reverse, suggesting a bigger move when the reversal finally comes.

---

## Support/Resistance Lines (Dashed)

When a setup completes (count reaches 9), a dashed S/R line is drawn:

- **Red dashed line** = Resistance level (high of the 1st bar in a sell setup)
- **Green dashed line** = Support level (low of the 1st bar in a buy setup)

**How to use:**
- If price stays below resistance after an MRI Top, the reversal is more likely
- If price stays above support after an MRI Bottom, the reversal is more likely
- If price breaks through the S/R line, the trend is continuing and extensions begin

---

## Breakout Lines (Blue Solid)

A solid blue line appears when price closes beyond an S/R level:

- Price closes **above** resistance = Bullish breakout (trend continuing up)
- Price closes **below** support = Bearish breakout (trend continuing down)

Breakout lines signal that the trend is strong and the MRI reversal signal did not hold.

---

## Extensions (A, B, C)

After a completed setup, if price continues in the trend direction (breaks S/R), extensions track 13 non-consecutive candles to find the next exhaustion point.

### Extension A
- **Sell:** Close > High of 2 bars ago
- **Buy:** Close < Low of 2 bars ago
- **Bar 13 qualifier:** Close of bar 13 must exceed close of bar 8

### Extension B
- **Sell:** Close > Close of 2 bars ago
- **Buy:** Close < Close of 2 bars ago
- **Bar 13 qualifier:** High/Low of bar 13 must exceed close of bar 8

### Extension C (Most Restrictive)
- **Sell:** Close > High of 2 bars ago AND Close > Close of 1 bar ago AND (for first 10 bars: High > High of 1 bar ago)
- **Buy:** Close < Low of 2 bars ago AND Close < Close of 1 bar ago AND (for first 10 bars: Low < Low of 1 bar ago)
- **Bar 13 qualifier:** Same as Extension B

**Extension labels:**
- Numbers 1-12 appear as the count progresses
- Letter **A**, **B**, or **C** appears when the extension completes (count 13 is qualified)
- **+** appears when count reaches 13 but the qualifier is not met (deferred)

**Extension cancellation:**
- Opposite MRI completion cancels all active extensions
- Price breaking the S/R line in the opposite direction cancels extensions

---

## Multi-Timeframe (MTF) Display

When MRI signals fire on higher timeframes, they appear as labels on the right side of the chart:

- Format: **TF,count** (e.g., "1D,1" means Daily timeframe has 1 consecutive MRI signal)
- When multiple timeframes align (e.g., Daily + Weekly both showing MRI signals), expect significant moves

**Available timeframes:** 1H, 1D, 1W, 1M, 12M (Yearly), plus 3 custom timeframes

---

## Settings

### Display Settings
- **Show Setup Numbers** — Toggle the 1-8 count display
- **Show MRI Top/Bottom Arrows** — Toggle the arrow signals at count 9
- **Show Consecutive Count** — Toggle the consecutive signal number

### Extension Settings
- **Extension Display** — Choose which extensions to show: All, A, B, C, B & C, or None

### Line Settings
- **Show Support/Resistance Lines** — Toggle S/R lines
- **Show Breakout Lines** — Toggle breakout lines
- **Max S/R Lines Visible** — How many lines to keep on chart (prevents chart compression)

### Multi-Timeframe Settings
- Enable/disable each timeframe
- Configure up to 3 custom timeframes

---

## Trading Tips

1. **Don't trade blindly on count 9** — Use it as a warning zone and confirm with candlestick patterns (shooting stars, hammers, dojis)
2. **The signal can be early or late by 1 candle** — This is normal behavior
3. **Best on Daily and Weekly timeframes** — More reliable signals on higher timeframes
4. **Watch for MTF alignment** — Multiple timeframes hitting 9 simultaneously = very strong signal
5. **Use 4H for entries, Daily/Weekly for direction**
6. **S/R lines are key** — If the S/R line holds after an MRI signal, the reversal is more probable
7. **Extensions B & C are most useful** — Tone Vays himself prefers B & C over A
8. **Higher consecutive counts = bigger potential moves** — A "3" or higher is historically significant

---

## Disclaimer

Trading is risky. MRI (like any indicator) does not guarantee positive returns. It does not blindly provide Buy/Sell/Short calls. The trader must evaluate every signal in context.

*"The average man doesn't wish to be told that it is a bull or a bear market. What he desires is to be told specifically which particular stock to buy or sell."* — Jesse Livermore
