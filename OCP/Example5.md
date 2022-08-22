### Usage

---
#### Where

https://github.com/tradingview/lightweight-charts/blob/master/src/formatters/percentage-formatter.ts#L3-L11


#### Why

class `PercentageFormatter` - extends base `PriceFormatter` class to reimplement `format()` method. So either `PercentageFormatter` or `PriceFormatter` can be used depending on a situation. One could say that `PricedFormatter` is closed for modification, but open for extension.

------------------------

### Violation

---
#### Where

https://github.com/BabylonJS/Babylon.js/blob/master/packages/dev/gui/src/2D/controls/button.ts

#### Why

Здесь слишком много уровней наследования для класса Button.

```
export class Button extends Rectangle {
class Rectangle extends Container
export class Container extends Control
```