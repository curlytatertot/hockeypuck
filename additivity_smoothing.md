# Data Smoothing / Additivity

### Lightkeeper calculates performance attribution over multi-period time intervals, and across multiple components (e.g. &#151; Long/Short or Market Cap).  To preserve the effects of compounding, adjustments are made to achieve additivity via data smoothing.

### Lightkeeper's chosen method of adjusting component retuns works over any number of simultaneous levels of component attribution, applied in arbitrary order.  This method is computationally transparent and supports interactive exploration.

| |Method|Example|
|1)|Start with  non-compounded/arithmetic returned.  | TOTAL: 10% = LONG: 7.5% + SHORT: 2.5%|
|Determine compounded and arithmetic returns of the complete portfolio for each time period | TOTAL COMPOUNDED: 8.0%|



