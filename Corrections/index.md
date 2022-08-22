# DIP
---
### Usage Example

### Where

https://github.com/angular/angular/blob/main/packages/language-service/src/references_and_rename.ts#L26

### Why

NgCompiler is Class, so ReferencesBuilder depends on implementation (not abstraction).

---

# LSP

---

### Violation Example

### Where

https://github.com/angular/angular/blob/main/packages/service-worker/worker/src/named-cache-storage.ts#L9

### Why

NamedCache extends parent interface Cache, so interface Cache is not overloaded.

---

### Violation Example

### Where

`Action`
https://github.com/BabylonJS/Babylon.js/blob/fdbf393d1d7699dc7cc69cec1dca0819ebd2622a/packages/dev/core/src/Actions/action.ts

`ExecuteCodeAction`
https://github.com/BabylonJS/Babylon.js/blob/fdbf393d1d7699dc7cc69cec1dca0819ebd2622a/packages/dev/core/src/Actions/directActions.ts#L489

### Why

execute method has stricter precondition in child class

---
