### Usage

---
#### Where

https://github.com/angular/angular/blob/main/packages/compiler-cli/integrationtest/src/jit_summaries.ts#L27

#### Why

Base is opened to be extended and closed to be changed.

------------------------

### Violation

---
#### Where

https://github.com/angular/angular/blob/main/packages/platform-browser/src/dom/dom_renderer.ts#L95

#### Why

The better way is to remove switch/case and extend DomRendererFactory2.
