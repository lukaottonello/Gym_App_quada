# Upper Body Hypertrophy v3 — PWA

**Quada Edition · Evidence-Based Training 2025**

Una Progressive Web App dark AMOLED per seguire il protocollo di ipertrofia upper body basato su evidenze scientifiche.

## Features

- **3 Sessioni**: G1 Heavy Push & Pull, G2 Arm Day, G3 Shoulder & Back
- **Doppia Progressione automatica**: suggerisce il peso per la prossima sessione
- **Timer di recupero** con Screen Wake Lock API (schermo sempre acceso)
- **Log nutrizionale**: tracking proteine e calorie con analisi distribuzione MPS
- **Calendario storico**: visualizzazione mensile dei workout e dell'aderenza nutrizionale
- **Libreria scientifica**: riferimenti alle ricerche di Schoenfeld, Maeo, Helms, Israetel
- **Offline-first**: Service Worker per uso senza internet
- **Installabile** su Android e iOS (PWA)
- **Export/Import** backup JSON

## Deploy rapido su GitHub Pages

1. Fork o upload di questi file nel tuo repository GitHub (public)
2. Settings → Pages → Branch: main / folder: / (root)
3. Attendi 1-2 minuti → `https://USERNAME.github.io/REPO-NAME/`

## Installazione sul telefono

**Android**: Chrome → menu 3 puntini → "Aggiungi a schermata Home"

**iPhone**: Safari → tasto Condividi → "Aggiungi a schermata Home"

## Struttura

```
├── index.html      # App completa (single-file)
├── sw.js           # Service Worker
├── manifest.json   # PWA manifest
└── README.md
```

## Aggiornamenti

Dopo ogni modifica a `index.html`, incrementa la versione della cache in `sw.js`:
```js
const CACHE_NAME = 'ubh-v3-cache-v2'; // cambia il numero
```

## Dati

Tutti i dati sono salvati in `localStorage` del browser. Usa "Esporta Backup JSON" per fare backup prima di cambiare device o browser.

## Riferimenti scientifici

- Schoenfeld BJ (2010, 2017) — meccanismi ipertrofia
- Israetel M et al. (2019) — MEV/MAV/MRV framework
- Maeo S et al. (2023) — ipertrofia tricipiti overhead +40%
- Helms ER et al. (2014) — proteine per natural bodybuilding
- Damas F et al. (2016) — frequenza e MPS
- Morton RW et al. (2018) — supplementazione proteica
- Meeusen R et al. (2013) — overtraining e deload

---

*Disclaimer: Questo programma è a scopo informativo. Consultare un medico prima di iniziare qualsiasi programma di allenamento intensivo.*
