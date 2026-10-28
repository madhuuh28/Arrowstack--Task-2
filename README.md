# Arrowstack Task 2 — AI Code Review & Optimization Assistant

A Python desktop app using Tkinter and Google's Gemini API. It reviews Python code as text, returns likely issues and recommendations, suggests optimizations, drafts improved code, and proposes tests.

## Run in VS Code (Windows)
1. Open this folder in VS Code and select Terminal → New Terminal.
2. Create an environment: `py -m venv .venv`
3. Activate in PowerShell: `.venv\\Scripts\\Activate.ps1`
4. Install packages: `python -m pip install -r requirements.txt`
5. Copy `.env.example` to a new file named `.env`.
6. Put your real key after `GEMINI_API_KEY=` in `.env`. Never commit or share this key.
7. Run: `python app.py`

You can alternatively paste your key into the masked API-key field in the app window.

## Safety
The submitted code is sent to Gemini as text and is not executed by this app. Do not submit confidential code unless authorized. AI suggestions can be wrong; test changes manually.
