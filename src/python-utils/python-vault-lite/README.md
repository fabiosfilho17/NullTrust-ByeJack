# python-vault-lite

A tiny local secrets vault for learning and future reuse in automation projects.

## Goals
- Store secrets encrypted at rest in a single file (`vault.enc.json`)
- Never store the master password
- Provide a small CLI: `init`, `set`, `get`, `list`

## Non-goals (v1)
- No cloud sync, no multi-user sharing, no rotation workflows
- No GUI
- No "enterprise vault" features

## Threat model (simple)
- Protect secrets if someone gets the repository/files but not the master password.
- If an attacker gets the master password (or you type it on a compromised machine), secrets are compromised.

## Quickstart
Create a venv and install dependencies:
```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt

