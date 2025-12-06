@"
# NAM Architecture

NAM — Naming Adaptation Module — является адаптивным слоем между ядром знаний (Knowledge Core), агентными системами и документами.

Он состоит из четырёх ключевых уровней:

---

## 1. Knowledge Base Layer
Структурированная база знаний NAM:

- онтология терминов;
- внутренние системные идентификаторы;
- профили заказчиков (default, industrial, gov, finance, healthcare, military);
- правила адаптации;
- стилистические модели;
- политика безопасности KB.

KB — это фундамент адаптации терминов.

---

## 2. Adaptation Engine Layer
Основной логический движок NAM:

- разрешение терминов (alias resolution);
- обработка конфликтов;
- генерация новых терминов;
- унификация стиля;
- управление профилями;
- интеграция с LLM (LLaMA).

Адаптер превращает системные ID в термины, согласованные с отраслью и клиентом.

---

## 3. API Layer
REST API поверх FastAPI:

- `/resolve/term`
- `/resolve/all`
- `/profiles/list`
- `/profile/set`
- `/validate/alias`
- `/security/check`

API позволяет интегрировать NAM в любые внешние системы:
MindForge, UAG, CRM, Helpdesk, OSINT.

---

## 4. Security Layer
NAM включает промышленную двухконтурную модель безопасности:

- внутренний контур (internal ID)
- внешний контур (adapted terminology)

Механизмы:
- контроль целостности KB;
- ACL и RBAC;
- политика редактирования;
- журналирование;
- audit trail.

---

## Архитектурная диаграмма

```mermaid
flowchart TD

A[Knowledge Base] --> B[Adaptation Engine]
B --> C[API Layer]
B --> D[Security Layer]

C --> E[External Systems]
D --> E
