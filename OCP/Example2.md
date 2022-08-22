### Usage

---
#### Where

https://github.com/withastro/astro/blob/f0f6a3332f88327cf165a35a668ca14aeaac0491/packages/webapi/src/lib/HTMLImageElement.ts

#### Why

Когда нам нужен новый функционал для HTMLElement, мы не меняем базовый класс, а наследуемся от него, переопределяя, добавляя новую функциональность(если нужно)

------------------------

### Violation

---
#### Where

https://github.com/tradingview/lightweight-charts/blob/master/src/model/pane.ts#L81-L94

#### Why

`priceScaleById` method of `Pane` class uses `switch` statement to define a price scale by a string id. At the moment there are only two possible price scales (left and right), but if there were a need to add some other variants (e.g. top, bottom), then modification of the `switch` statement would have been done, and this would result in violation of "closed for modification" principle. Either inheritance or an interface could be used to avoid the problem.