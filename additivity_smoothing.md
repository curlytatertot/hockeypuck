# Data Smoothing / Additivity

### Lightkeeper calculates performance attribution over multi-period time intervals, and across multiple components (e.g. &#151; Long/Short or Market Cap).  To preserve the effects of compounding, adjustments are made to achieve additivity via data smoothing.

### Lightkeeper's chosen method of adjusting component retuns works over any number of simultaneous levels of component attribution, applied in arbitrary order.  This method is computationally transparent and supports interactive exploration.

| |Method|Example|
|:----|----|----|
|1)|Start with  non-compounded/arithmetic returned.  | **Arithmetic Returns:**<BR>TOTAL: 10% = LONG: 7.5% + SHORT: 2.5%|
|2)|Determine compounded and arithmetic returns of the complete portfolio for each time period | **TOTAL COMPOUNDED:** 8.0%|
|3)|Calculate the adjustment factor, the raio of the compounded and arthmetic returns| 8.0% / 10% = 0.8|
|4)|Multiply adjustment factor into arithmetic returns to get adjusted returns|**Adjusted Component Return:**<BR> Long (adj) = 7.5% x 0.8 = 6.0%<BR> Short (adj) = 2.5% x 0.8 = 2.0%<BR> **Adjusted Return:**<BR>6.0% + 2.0% = 8.0%|

#### _Caveat: The interpretation of attributions should be treated carefully when time periods span periods of large and sudden variation in the underlying basis used in the return calculation._

For a comprehensive summary of methodologies used for adjusting component returns to achieve additivity: _Multiperiod Arithmetic Attribution_, Jose Menchero, Financial Analysts Journal, Volume 60, Number 4, 2004, CFA Institute

#### [Illustrated: Download PDF &#151; Data Smoothing: Additivity](www.lightkeeper.com/gitbook/Lightkeeper_Additivity.pdf)
