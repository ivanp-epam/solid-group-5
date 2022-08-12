### Usage

---
#### Where
https://github.com/keycloak/keycloak/blob/89795cfd7df24aad392c6223fe6d4639f03bd03d/core/src/main/java/org/keycloak/exceptions/TokenVerificationException.java#L27

#### Why

Правильная иерархия классов, закрыт для изменения, открыт для расширения

------------------------

### Violation

---
#### Where

https://github.com/keycloak/keycloak/blob/89795cfd7df24aad392c6223fe6d4639f03bd03d/core/src/main/java/org/keycloak/TokenVerifier.java#L430

#### Why

В такой реализации есть вероятность, что метод надо будет дописывать