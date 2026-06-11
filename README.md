# Lama Pro 🦙

Ein persönlicher KI-Assistent auf Basis der **NVIDIA NIM API**, verfügbar als Desktop-App (Windows), mobile Web-App und eigenständige Android-App.

## Features

- **4 Modi**:
  - ⚡ **Schnell** – kurze, schnelle Antworten (`meta/llama-3.1-8b-instruct`)
  - 💬 **Standard** – allgemeiner Assistent (`meta/llama-3.3-70b-instruct`)
  - 💻 **Code** – Programmieren & Debuggen (`nvidia/llama-3.3-nemotron-super-49b-v1`)
  - 🎨 **Bilder** – Bildgenerierung (`black-forest-labs/flux.1-dev`)
- Verlauf wird lokal gespeichert (Chats & generierte Bilder)
- Drei Plattformen aus einer Codebasis:
  - **Desktop** (`src/main.py` / `Lama Pro.exe`) – customtkinter-Oberfläche für Windows
  - **Web** (`src/web_server.py` + `src/web/`) – mobile-freundliche Weboberfläche, im selben WLAN vom Smartphone erreichbar
  - **Android** (`mobile/`) – eigenständige APK, spricht direkt mit der NVIDIA-API (kein PC nötig)


## Download

Fertige Builds können unter [`releases/`](releases/) (jeweils nach Version sortiert) gefunden werden. Vorab-Versionen können unter [`prereleases/`](prereleases/) gefunden werden.


### 2. Desktop-App

```bash
pip install -r requirements.txt
python src/main.py
```

Fertige Windows-EXE: siehe [`releases/`](releases/).

### 3. Mobile Web-App

```bash
scripts\start_web.bat
```

Zeigt eine Adresse wie `http://192.168.x.x:5000` an – im Handy-Browser (selbes WLAN) öffnen.

### 4. Android-APK

Die APK in [`releases/`](releases/) ist eigenständig und benötigt keinen laufenden PC – sie spricht direkt mit der NVIDIA-API. Einfach installieren ("Installation aus unbekannten Quellen" ggf. erlauben) und öffnen.


## Versionierung

Aktuelle Version: siehe [`VERSION`](https://github.com/VortexStudiosLab/Lama-Pro/blob/main/VERSION.txt). Änderungen siehe [`CHANGELOG.md`](https://github.com/VortexStudiosLab/Lama-Pro/blob/main/CHANGELOG.md).
