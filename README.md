# NAM — Naming Adaptation Module
Adaptive Naming System for Knowledge Engines, Agents, Pipelines, Documents, and Architectures

NAM — промышленный модуль адаптивной терминологии, обеспечивающий:
- подмену терминов под отраслевой профиль,
- поддержку разных заказчиков без изменения ядра,
- адаптацию документов, KB, ролей и интерфейсов,
- интеграцию с AI-агентами,
- API для внешних систем,
- поддержание двухконтурной модели безопасности.

NAM входит в платформу MindForge и совместим с:
- UAG (Universal Agent Gateway)
- KM-6 Reasoning Engine
- OSINT Fabric
- MSDLC Pipeline

---

## 📘 Основные возможности
- 🔄 Адаптация терминов: industrial, government, finance, military, healthcare
- 📚 Онтология NAM
- 🧩 Профили заказчиков
- 🔧 API-слой для интеграции
- 🛡 Двухконтурная безопасность
- 📑 Контроль целостности KB
- 🧾 Аудит действий

---

## 🚀 Быстрый запуск API
```
pip install -r requirements.txt
uvicorn src.api.server:app --reload
```

---

## 🔗 Основные API endpoints
- POST /resolve/term
- POST /resolve/all
- GET  /profiles/list
- POST /profiles/set
- POST /security/check
- POST /validate/alias

Описание API — `docs/api/NAM_API_SPEC.md`.

---

## 🧩 Архитектура NAM
```
MindForge Platform
   ├── Knowledge Core
   ├── KM-6 Reasoning Engine
   ├── UAG InterAgent Protocol
   ├── OSINT Fabric
   └── NAM — Naming Adaptation Layer
```

---

## 📜 Лицензия
MIT License © 2025 Victor Kulichenko
