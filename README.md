# NSOL BPO Call Assistant

This repository contains the same source files as [Lk-Agent-System](https://github.com/ishahzaibarshad/Lk-Agent-System), including the FastAPI call-management service, scripted LiveKit agent, dashboards, and SQLite setup. It is a duplicate copy of that project rather than a separate frontend-only implementation.

The source includes Twilio call and webhook routes, a scripted qualification and scheduling conversation, an HTML dashboard, and an optional Streamlit interface. The existing run guide says that the Twilio media-stream-to-LiveKit audio connection remains to be completed; verify that path before presenting this as a fully working voice-calling system.

Install dependencies with `pip install -r requirements.txt`, configure service credentials locally, then start the API using the project startup script or `uvicorn main:app --host 0.0.0.0 --port 8000`. The optional Streamlit interface is launched with `streamlit run streamlit_app.py`.

Do not deploy with sample credentials. Rotate exposed provider tokens, replace any default account credentials, and keep `.env` files out of Git.

**Portfolio note:** Because this repository currently duplicates `Lk-Agent-System`, feature one canonical copy rather than presenting both as separate projects.

