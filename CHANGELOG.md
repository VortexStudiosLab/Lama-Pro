# Changelog

Alle nennenswerten Änderungen an Lama Pro werden in dieser Datei dokumentiert.

## v.1.0.0 - 2026-06-11

### Added
- Desktop-App (customtkinter) mit 4 Modi: Schnell, Standard, Code, Bilder
- Anbindung an die NVIDIA NIM API (Chat-Streaming + Bildgenerierung)
- Lokale Persistenz von Chatverläufen und generierten Bildern
- Einstellungsdialog für API-Key und Modell-IDs
- Mobile Web-App (Flask-Server + responsive Oberfläche) für den Zugriff vom Smartphone im selben WLAN
- Eigenständige Android-App (APK), die direkt mit der NVIDIA-API kommuniziert (kein PC nötig)
- Windows-EXE-Build via PyInstaller

### Changed
- Bildgenerierungsmodell von `stabilityai/stable-diffusion-3.5-large` (nicht mehr verfügbar) auf
  `black-forest-labs/flux.1-schnell`, später auf `black-forest-labs/flux.1-dev` (höhere Qualität, 30 Schritte)
- Code-Modell von `qwen/qwen2.5-coder-32b-instruct` (End-of-Life) auf `nvidia/llama-3.3-nemotron-super-49b-v1`

### Fixed
- Speichern-Button im Einstellungsdialog war durch ein zu kleines Fenster nicht sichtbar
- CORS-Unterstützung für die mobile Web-App ergänzt
- Zuverlässiges Senden von Nachrichten in der Android-App über native HTTP-Requests (CapacitorHttp)
