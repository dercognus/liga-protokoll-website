# Liga Wettkampf Website

Öffentliche Website für Trampolin Liga-Wettkampf-Protokolle.

## Übersicht

Diese statische Website hostet automatisch hochgeladene Wettkampf-Protokolle von der Liga-Protokoll-App.

## Struktur

```
liga-wettkampf-website/
├── public/
│   ├── index.html          # Übersichtsseite mit Wettkampf-Liste
│   ├── styles.css          # Styling
│   └── competition-X/      # Automatisch hochgeladen von der App
│       ├── protokoll.html  # Detailliertes Protokoll
│       └── index.html      # Wettkampf-Übersicht
├── vercel.json             # Vercel-Konfiguration
└── package.json
```

## Deployment

Die Website wird automatisch von Vercel deployed bei jedem Push zu `main`.

## Automatischer Upload

Die Liga-Protokoll-App lädt Wettkampf-Protokolle automatisch via GitHub API hoch.

**Setup:**
1. GitHub Personal Access Token generieren (`repo` Scope)
2. Token in der Liga-Protokoll-App unter "Einstellungen → GitHub-Upload" eintragen
3. Nach jeder finalen Wertung werden Protokolle automatisch hochgeladen

## Lokale Entwicklung

```bash
# Vercel CLI installieren (optional)
npm install -g vercel

# Lokalen Dev-Server starten
vercel dev
```

## Lizenz

Private Projekt für Liga-Wettkämpfe
