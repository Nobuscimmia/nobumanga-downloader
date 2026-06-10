# 🈳 NobumangaDownloader

**Il modo più semplice per scaricare e gestire i tuoi manga preferiti su Windows.**

![Version](https://img.shields.io/badge/version-1.0.0-red)
![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-blue)
![Python](https://img.shields.io/badge/python-3.11+-green)

---

## ✨ Funzionalità

- 🔍 **Ricerca manga** per titolo o URL diretto da MangaWorld
- ⬇️ **Download parallelo** di più capitoli contemporaneamente
- 📚 **Libreria locale** con copertine e stato avanzamento
- 📖 **Lettore integrato** CBZ/ZIP con zoom e navigazione da tastiera
- 🗂️ **Raggruppamento in volumi** (es. cap. 1–10 → Volume 01.cbz)
- 💾 **Esporta in PDF, CBZ, ZIP o JPG**
- ⏰ **Download automatico notturno** — controlla nuovi capitoli ogni notte
- 🔔 **Notifiche Windows** quando un download o volume è pronto
- 🔄 **Auto-aggiornamento** — notifica quando esce una nuova versione

---

## 🚀 Installazione (utente finale)

1. Scarica `NobumangaDownloader_Setup_v1.0.0.exe` dalla pagina [Releases](https://github.com/nobuscimmia/nobumanga-downloader/releases)
2. Esegui il setup e segui le istruzioni
3. Avvia NobumangaDownloader dal desktop o dal menu Start

**Requisiti:** Windows 10/11 (64-bit) · Connessione internet

---

## 🛠️ Build da sorgente

### Prerequisiti
```
Python 3.11+
pip install -r requirements.txt
pip install pyinstaller
```

### Build exe
```bash
# Windows — doppio click su build.bat oppure:
pyinstaller build.spec --clean

# Output: dist\NobumangaDownloader.exe
```

### Installer (opzionale)
1. Installa [Inno Setup](https://jrsoftware.org/isinfo.php)
2. Apri `installer.iss` con Inno Setup
3. **Build → Compile**
4. Output: `installer_output\NobumangaDownloader_Setup_v1.0.0.exe`

---

## 📁 Struttura progetto

```
NobumangaDownloader/
├── main.py              # Entry point
├── build.spec           # Config PyInstaller
├── build.bat            # Script build Windows
├── installer.iss        # Config Inno Setup
├── version.json         # Versione per auto-update
├── requirements.txt
├── gui/
│   ├── app.py           # Finestra principale
│   ├── splash.py        # Splash screen animato
│   └── tabs/            # Search, Download, Library, Viewer, Settings
├── core/
│   ├── scraper.py       # Scraping MangaWorld
│   ├── downloader.py    # Download asincrono
│   ├── converter.py     # CBZ / PDF / ZIP
│   ├── library.py       # SQLite locale
│   ├── scheduler.py     # Aggiornamenti automatici
│   ├── notifier.py      # Notifiche Windows
│   └── updater.py       # Auto-aggiornamento
└── assets/
    ├── icon.ico
    ├── icon.png
    └── splash.png
```

---

## 📄 Licenza

Uso personale. Vedere [LICENSE](LICENSE) per i dettagli.  
I contenuti scaricati sono soggetti ai termini di MangaWorld.

---

*Sviluppato da [Nobuscimmia](https://gumroad.com/nobuscimmia)*
