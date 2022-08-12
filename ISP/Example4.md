### Usage

---
#### Where

https://github.com/tradingview/lightweight-charts/blob/master/src/views/pane/iupdatable-pane-view.ts#L5-L7

#### Why

interface `IUpdatablePaneView` extends `IPaneView` adding `update` method. So if some pane view should be updatable, more specific interface can be used, but if there is no such need, simple `IPaneView` can be used. Such approach relieves classes of implementation of `update` method in case they do not need it.

------------------------

### Violation

---
#### Where

None

#### Why

None