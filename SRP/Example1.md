### Usage

---
#### Where

https://github.com/microsoft/vscode/blob/main/src/vs/editor/common/core/editOperation.ts

#### Why

https://github.com/microsoft/vscode/blob/main/src/vs/editor/common/core/editOperation.ts

------------------------

### Violation

#### Where

https://github.com/angular/angular/blob/main/packages/router/src/router.ts#L371

#### Why

Router is too clever. I would suggest to split it into NavigationExecuter and NavigationGuards classes and move logic of setupNavigations there.
