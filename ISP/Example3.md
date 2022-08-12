### Usage

---
#### Where

None

#### Why

None

------------------------

### Violation

---
#### Where
https://github.com/tradingview/lightweight-charts/blob/master/src/gui/mouse-event-handler.ts#L13-L41 

#### Why

`MouseEventHandlers` is quite large. Contrary to its name, it deals not only with mouse events, but also taps and pinches. It could be split into two or more interfaces (e.g. `MouseEventHandlers` and `TouchGesturesHandlers`).