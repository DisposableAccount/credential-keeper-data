# Credential Keeper requirements catalog

`requirements.json` is the list of state board, certifying board and credential renewal rules that the
Credential Keeper app checks for every 90 days. The app reads it from:

https://raw.githubusercontent.com/DisposableAccount/credential-keeper-data/main/requirements.json

Users only see a change when they accept it on each credential. Raise `version` on every update; the app
ignores a file whose version isn't newer than the one it has.

Source of truth: `tools/build_catalog.py` in the app project. Rebuild there, then upload the new
`requirements.json` here (or run `tools/publish_catalog.sh`).
