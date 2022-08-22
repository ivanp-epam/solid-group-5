### Usage

---
#### Where

https://github.com/angular/angular/blob/main/packages/platform-server/src/domino_adapter.ts#L41

#### Why

Method setRootDomAdapter takes adapter (type - DomAdapter). So BrowserDomAdapter can be easily replaced with DominoAdapter as we can see: https://github.com/angular/angular/blob/main/packages/platform-browser/src/browser/browser_adapter.ts#L22

------------------------

### Violation

---
#### Where

https://github.com/tradingview/lightweight-charts/blob/master/src/api/candlestick-series-api.ts#L8-L13 

#### Why

class `CandlestickSeriesApi` takes more specific arguments in `applyOptions` method than the base class - preconditions for the method are tightened. If we swapped the base class usage with it, it might potentially break the application.