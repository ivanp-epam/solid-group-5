### Usage

---
#### Where

https://github.com/microsoft/vscode/blob/main/src/vs/workbench/common/component.ts#L17 

#### Why

Класс Component не зависит от класса storageService(класса нижнего уровня), который он использует, вместо этого он принимает объект реализующий IStorageService то есть зависит от абстракции

------------------------

### Violation

---
#### Where

None

#### Why

None