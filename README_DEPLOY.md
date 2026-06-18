# 🚀 MUMTY Brand Discovery Tool – Deployment-Anleitung

Dein Personal-Brand-Tool in ca. 10 Minuten live – kostenlos, sicher, professionell.

---

## Was du brauchst

- [ ] Einen **GitHub-Account** (kostenlos) → https://github.com
- [ ] Einen **Vercel-Account** (kostenlos) → https://vercel.com
- [ ] Deinen **Anthropic API Key** aus der Claude Console

---

## Schritt 1 – Dateien auf GitHub hochladen

1. Gehe zu https://github.com → **„New repository"**
2. Name z. B. `mumty-brand-tool` → **Public** oder **Private** → **„Create repository"**
3. Klicke auf **„uploading an existing file"**
4. Lade diese Ordnerstruktur hoch:

```
mumty-brand-tool/
├── api/
│   └── claude.js        ← der sichere API-Proxy
├── public/
│   └── index.html       ← dein Brand-Tool
└── vercel.json          ← Konfiguration
```

5. Klicke **„Commit changes"** → fertig!

---

## Schritt 2 – Mit Vercel verbinden

1. Gehe zu https://vercel.com → **„Add New Project"**
2. Klicke **„Import Git Repository"** → wähle dein `mumty-brand-tool` Repo
3. Alles auf Standard lassen → **„Deploy"** klicken
4. Vercel deployt automatisch – dauert ca. 30 Sekunden

---

## Schritt 3 – API Key sicher hinterlegen ⚠️

Das ist der wichtigste Schritt! Den Key NIEMALS in den Code schreiben.

1. In Vercel: Gehe zu deinem Projekt → **„Settings"** → **„Environment Variables"**
2. Klicke **„Add New"**
3. **Name:** `ANTHROPIC_API_KEY`
4. **Value:** Deinen Key einfügen (beginnt mit `sk-ant-...`)
5. **„Save"** klicken
6. Danach: **„Deployments"** → **„Redeploy"** (damit der Key aktiv wird)

---

## Schritt 4 – Deine URL teilen

Nach dem Deploy bekommst du eine URL wie:
`https://mumty-brand-tool.vercel.app`

Diese URL kannst du:
- Als **Link in deinem Linktree** (linktr.ee/mumtybymiri) eintragen
- Als **Freebie** per E-Mail verschicken
- Als **Low-Ticket Mini-Produkt** (z. B. 9–27 €) verkaufen
- In deiner **Instagram Bio** verlinken

---

## Kosten

| Was | Kosten |
|-----|--------|
| GitHub | Kostenlos |
| Vercel Hosting | Kostenlos (bis 100 GB/Monat) |
| Anthropic API | Ca. 0,01–0,03 € pro Nutzung (Sonnet 4.6) |

Bei 100 Nutzerinnen pro Monat: ca. 1–3 € API-Kosten.

---

## Optional: Eigene Domain

Wenn du `brand.mumty.de` möchtest statt der Vercel-URL:

1. Vercel → Projekt → **„Domains"** → **„Add Domain"**
2. `brand.mumty.de` eingeben
3. Bei IONOS (deinem Hoster): einen CNAME-Eintrag auf `cname.vercel-dns.com` setzen
4. Fertig – dauert ca. 10 Minuten bis die Domain aktiv ist

---

## Nutzungslimit schützen (empfohlen)

Damit keine unbekannten Personen dein Tool unbegrenzt nutzen:

Gehe in der Anthropic Console unter **„Limits"** und setze ein monatliches Budget-Limit
(z. B. 10 € als Sicherheitsnetz).

→ https://console.anthropic.com

---

## Probleme?

| Fehler | Lösung |
|--------|--------|
| „API Key nicht konfiguriert" | Environment Variable in Vercel prüfen + Redeploy |
| Tool lädt aber KI antwortet nicht | API Key in Console prüfen ob aktiv |
| 404 auf `/api/claude` | `vercel.json` prüfen ob hochgeladen |

---

Bei Fragen: miriamstark.mumty auf Instagram 🌿
