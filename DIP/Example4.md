### Usage

---
#### Where

https://github.com/tradingview/lightweight-charts/blob/master/src/gui/mouse-event-handler.ts#L158-L162

#### Why

class `MouseEventHandler` depends on abstractions `MouseEventHandlers`, `MouseEventHandlerOptions` and does not depend on actual implementations. Any class complying with an interface can be provided.

------------------------

### Violation

---
#### Where

https://github.com/tradingview/lightweight-charts/blob/master/src/formatters/date-time-formatter.ts#L18-L33

#### Why

class `DateTimeFormatter` - high-level class depends on implementations (`DateFormatter` and `TimeFormatter`) instead of an interface. `Formatter` interface with `format()` method could be created and used here instead.