### Usage

---
#### Where

https://github.com/photonstorm/phaser/blob/master/src/cache/BaseCache.js

#### Why

Класс BaseCache https://github.com/photonstorm/phaser/blob/master/src/cache/BaseCache.js использует EventEmiter и помогает сделать его абстрактным для остальных частей приложения. Если  EventEmitter (third-party library) изменится, нам нужно будет заменить его только в классе BaseCache

------------------------

### Violation

---
#### Where

https://github.com/angular/angular/blob/main/packages/compiler-cli/src/ngtsc/metadata/src/util.ts#L202

#### Why

MetadataReader should be a base class and have only abstract method getData.
