NAM/
├── README.md
├── LICENSE
├── .gitignore
│
├── docs/
│   ├── architecture/ARCH_NAM.md
│   ├── api/NAM_API_SPEC.md
│   ├── security/
│   │   ├── SECURITY_MODEL.md
│   │   ├── DUAL_CONTOUR.md
│   │   ├── ACCESS_CONTROL.yaml
│   │   ├── INTEGRITY_POLICY.md
│   │   └── AUDIT_EVENTS.md
│   └── kb/KB_OVERVIEW.md
│
├── kb/
│   ├── 00_core/
│   │   ├── ontology.yaml
│   │   ├── entities.yaml
│   │   ├── roles.yaml
│   │   └── manifest.yaml
│   │
│   ├── 01_profiles/
│   │   ├── default.yaml
│   │   ├── industrial.yaml
│   │   ├── government.yaml
│   │   ├── finance.yaml
│   │   ├── healthcare.yaml
│   │   └── military.yaml
│   │
│   ├── 02_rules/
│   │   ├── alias_resolution.md
│   │   ├── style_guides.md
│   │   ├── collision_rules.md
│   │   └── validation.md
│   │
│   └── 03_security/
│       ├── redaction_rules.md
│       ├── token_policy.yaml
│       ├── integrity_checks.yaml
│       └── audit_config.yaml
│
├── src/
│   ├── api/
│   │   ├── server.py
│   │   └── routers/
│   │       ├── resolve.py
│   │       ├── profiles.py
│   │       └── security.py
│   │
│   ├── core/
│   │   ├── loader.py
│   │   ├── adapter.py
│   │   ├── validator.py
│   │   └── security.py
│   │
│   └── utils/
│       ├── hashing.py
│       ├── audit.py
│       └── logger.py
│
├── requirements.txt
└── NAM_PROMPT_v1.0.md
