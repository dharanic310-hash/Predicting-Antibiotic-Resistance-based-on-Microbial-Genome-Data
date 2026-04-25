backend/
│
├── app/
│   │
│   ├── main.py                 # FastAPI entry point
│   │
│   ├── core/                   # Core configurations
│   │   ├── config.py           # App settings
│   │   ├── security.py         # JWT, password hashing
│   │   └── dependencies.py     # Common dependencies
│   │
│   ├── database/
│   │   ├── db.py               # SQLite connection
│   │   ├── base.py             # Base for SQLAlchemy models
│   │   └── session.py          # DB session handler
│   │
│   ├── models/                 # Database tables
│   │   ├── user.py             # User table
│   │   ├── role.py             # Roles (doctor, technician, user)
│   │   ├── bacteria.py         # Bacteria info
│   │   ├── prediction.py       # Prediction history
│   │   └── antibiotic.py       # Antibiotic metadata
│   │
│   ├── schemas/                # Request/response validation
│   │   ├── user.py
│   │   ├── auth.py
│   │   ├── bacteria.py
│   │   ├── prediction.py
│   │   └── antibiotic.py
│   │
│   ├── routers/                # API endpoints
│   │   ├── auth.py             # Login / Register
│   │   ├── users.py            # User operations
│   │   ├── bacteria.py         # BV-BRC / NCBI fetch
│   │   ├── prediction.py       # Antibiotic prediction
│   │   ├── compare.py          # Compare antibiotics
│   │   └── admin.py            # Admin-only APIs
│   │
│   ├── services/               # Business logic
│   │   ├── auth_service.py
│   │   ├── bacteria_service.py
│   │   ├── prediction_service.py
│   │   └── ml_service.py
│   │
│   ├── ml_models/              # Saved ML models
│   │   ├── ampicillin.pkl
│   │   ├── ciprofloxacin.pkl
│   │   └── metadata.json
│   │
│   ├── utils/                  # Helper functions
│   │   ├── encoders.py
│   │   ├── preprocess.py
│   │   └── validators.py
│   │
│   └── __init__.py
│
├── app.db                      # SQLite database
├── requirements.txt
└── README.md
