### Usage

---
#### Where

https://github.com/keycloak/keycloak/blob/89795cfd7df24aad392c6223fe6d4639f03bd03d/core/src/main/java/org/keycloak/TokenIdGenerator.java#L27

#### Why

Класс занимается только генерацией id

------------------------

### Violation

---
#### Where

https://github.com/keycloak/keycloak/blob/89795cfd7df24aad392c6223fe6d4639f03bd03d/core/src/main/java/org/keycloak/TokenVerifier.java#L44

#### Why

Класс выполняет слишком много функций (верификация, опции с проверкой/без проверки, сбор данных, создание различных инстансов)