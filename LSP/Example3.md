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

https://github.com/angular/angular/blob/main/packages/platform-server/src/domino_adapter.ts#L79

#### Why

getBaseHref returns string, but in the parent class in returns string | null
