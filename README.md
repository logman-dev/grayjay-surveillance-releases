# Gray Jay Surveillance - Desktop Releases

Auto-update feed and installers for the Gray Jay Surveillance desktop app
(ROW surveillance, formerly "Grayjay Drone Desktop").

The application code lives in a private repository; this repo only hosts
release artifacts. Each release carries:

- `Gray-Jay-Surveillance_<version>_x64-setup.exe` - the Windows installer
- `latest.json` - the Tauri updater manifest (version, notes, Ed25519 signature, installer URL)

The app polls `releases/latest/download/latest.json` and only installs an
update whose signature matches the public key built into the app.
