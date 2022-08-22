### Usage

---
#### Where

https://github.com/tradingview/lightweight-charts/blob/master/src/formatters/percentage-formatter.ts#L3-L11

#### Why

class `PercentageFormatter` - we can safely swap usage of `PriceFormatter` with `PercentageFormatter`. The code will not break since the contract is respected.

------------------------

### Violation

---
#### Where

https://github.com/BabylonJS/Babylon.js/blob/master/packages/dev/core/src/Engines/engine.ts

#### Why

Violation: Суперкласс Engine: https://github.com/BabylonJS/Babylon.js/blob/master/packages/dev/core/src/Engines/engine.ts содержит ВСЕ МЕТОДЫ НА СВЕТЕ, от обработки текстур до выхода из полногоэкранного режима. Это God object.
