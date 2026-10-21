Townlight Utilities

Townlight Utilities v0.1.1 ships utility customer-service copilot foundations: cited utility-policy Q&A, CSR-safe read-only account context, payment-arrangement draft support, service-request intake, optional database-backed account/service workpapers, FastAPI runtime, public sample UI, docs, tests, browser QA, and release gates.

Optional workpaper persistence: set CIVICUTILITY_WORKPAPER_DB_URL to a SQLAlchemy database URL to store CSR-safe account snapshots and service-request intake drafts. Without it, POST endpoints stay stateless and retrieval endpoints explain how to enable storage.

It is not a utility billing system, payment processor, rate engine, shutoff/reconnect workflow, system of record, live LLM runtime, live billing connector, or Townlight 311 write-back integration.

Install:
python -m pip install -e ".[dev]"
python -m uvicorn civicutility.main:app --host 127.0.0.1 --port 8142

Townlight Utilities v0.1.1 is pinned to civiccore==0.3.0.

License: Code: AGPL-3.0-only, with the TownLight Public Institution Exception for qualifying deployments. See LICENSE and LICENSE-EXCEPTION.md. Documentation: CC BY 4.0 (LICENSE-DOCS).
