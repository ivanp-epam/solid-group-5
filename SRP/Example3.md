### Usage

---
#### Where

https://github.com/tradingview/lightweight-charts/blob/master/src/formatters/date-time-formatter.ts#L18-L33

#### Why

class `DateTimeFormatter` is only responsible for presenting datetime string. It uses lower level`DateFormatter` and `TimeFormatter` classes, both of which are only concerned with formatting their part of the string (date and time, respectively). 

------------------------

### Violation

---
#### Where

https://github.com/tradingview/lightweight-charts/blob/master/src/model/chart-model.ts#L337-L932

#### Why

`ChartModel` looks like a God object and implements 68 public methods. It could be split into several smaller classes.