# 📋 Istruzioni per pubblicare le classifiche

Questo documento spiega **come aggiornare la classifica del circuito** quando ricevi i risultati di una gara dal cronometraggio.

L'app è online a `https://fringuello79.github.io/atrs/` e legge automaticamente i file Excel pubblicati nella cartella `/classifiche/` di questo repository. Quando carichi un file con il nome corretto, **tutti i visitatori vedono subito la classifica aggiornata**, senza dover fare nulla.

---

## 🎯 Procedura veloce (3 passaggi)

1. **Ricevi** il file Excel dal cronometraggio
2. **Rinominalo** con il nome esatto della tabella qui sotto
3. **Caricalo** nella cartella `classifiche/` di questo repository su GitHub

L'app si aggiorna automaticamente entro pochi secondi.

---

## 📛 Tabella nomi file (IMPORTANTE — usa esattamente questi)

I nomi devono essere scritti **esattamente** come indicato: tutto minuscolo, con il trattino, senza spazi, senza accenti, estensione `.xlsx`.

### Skyrace del Voltigno (3 maggio 2026)

| Distanza | Nome file |
|---|---|
| Skyrun 19 km | `voltigno-19km.xlsx` |
| Skymarathon 34 km | `voltigno-34km.xlsx` |

### Alba dei Marsi (7 giugno 2026)

| Distanza | Nome file |
|---|---|
| Trail Corto 12 km | `alba-12km.xlsx` |
| Trail Lungo 21 km | `alba-21km.xlsx` |

### Skyrace del Mammut (21 giugno 2026)

| Distanza | Nome file |
|---|---|
| Trail del Mammut 12.4 km | `mammut-12km.xlsx` |
| Skyrace del Mammut 21 km | `mammut-21km.xlsx` |

### XTERRA Abruzzo Trail Run (18-19 luglio 2026)

| Distanza | Nome file |
|---|---|
| Urban Trail 10 km | `xterra-10km.xlsx` |
| Half Marathon 25 km | `xterra-25km.xlsx` |
| Marathon 41 km | `xterra-41km.xlsx` |

### Gran Sasso Trail (30 agosto 2026)

| Distanza | Nome file |
|---|---|
| Pietracamela Trail 11 km | `gransasso-11km.xlsx` |
| Madonnina Trail 21 km | `gransasso-21km.xlsx` |
| Trail del Gigante 40 km | `gransasso-40km.xlsx` |

### Skyrace del Maglio (18 ottobre 2026)

| Distanza | Nome file |
|---|---|
| SRM 30 km | `maglio-30km.xlsx` |

**Totale: 13 file da pubblicare durante la stagione.**

---

## 📤 Come caricare un file su GitHub

### Da computer

1. Vai su `https://github.com/fringuello79/atrs`
2. Apri la cartella `classifiche/` (cliccala)
3. Clicca **"Add file" → "Upload files"** in alto a destra
4. Trascina il file Excel rinominato nella zona di upload
5. In basso scrivi un messaggio breve, esempio: *"Aggiunta classifica Voltigno 19km"*
6. Clicca **"Commit changes"**

Pronto. L'app si aggiorna entro pochi secondi.

### Da telefono (iPhone/Android)

GitHub funziona anche da browser mobile, ma il modo più comodo è installare l'app **GitHub Mobile** (gratuita su App Store / Play Store):

1. Apri l'app GitHub e accedi
2. Vai al repository `atrs` → cartella `classifiche/`
3. Tocca i tre puntini in alto → **"Add file"** → seleziona il file Excel dalla galleria/file
4. Scrivi un messaggio commit e tocca **"Commit"**

---

## 🔄 Come sostituire un file già caricato

Esempio: hai caricato `voltigno-19km.xlsx` ma il cronometraggio ti manda una versione corretta.

1. Vai nella cartella `classifiche/` su GitHub
2. **Clicca sul file esistente** (`voltigno-19km.xlsx`)
3. Clicca l'icona della **matita** ✏️ in alto a destra (oppure il menù ⋯ → "Edit file"). Se la matita non appare, c'è anche **"Upload file"** sopra: caricare un file con lo stesso nome lo sovrascrive.
4. Conferma il commit

Il file viene sovrascritto e l'app si aggiorna automaticamente.

> ⚠️ **Cache del browser**: l'app usa un meccanismo "cache-busting" che forza il browser a riscaricare i file ogni volta. Se per qualche motivo un visitatore vede una classifica vecchia, basta che faccia un **refresh forzato**: `Ctrl+F5` (Windows), `Cmd+Shift+R` (Mac), oppure tirare giù la pagina sul mobile.

---

## ❌ Come rimuovere un file

Se hai caricato un file per errore:

1. Vai nella cartella `classifiche/`
2. Clicca sul file
3. Clicca il **cestino** 🗑️ in alto a destra (oppure menù ⋯ → "Delete file")
4. Conferma

L'app, alla ricarica, semplicemente non mostrerà più quella gara.

---

## 📊 Formato Excel atteso

I file Excel del cronometraggio devono contenere queste colonne (l'ordine non conta, l'app le riconosce automaticamente):

| Colonna richiesta | Varianti accettate dall'app |
|---|---|
| **Family Name** (obbligatoria) | `Family Name`, `Cognome`, `Surname`, `Last Name` |
| **First Name** (obbligatoria) | `First Name`, `Nome`, `Given Name` |
| Ranking / Posizione | `Ranking`, `Pos`, `Posizione` |
| Time / Tempo | `Time`, `Tempo` |
| Gender / Sesso | `Gender`, `Sesso`, `Sex` |
| BirthDate / Data nascita | `BirthDate`, `Birth`, `Nascita`, `DOB` |
| Team / Società | `Team`, `Società`, `Club` |
| ITRA ID, Bib, City | opzionali |

**Solo Cognome e Nome sono indispensabili.** Tutto il resto è "best effort": se mancano alcune colonne, l'app continua a funzionare comunque.

L'app prende automaticamente il **primo foglio** del file Excel. Se il cronometraggio ti manda un file con più fogli, assicurati che la classifica sia nel primo (oppure copia i dati in un nuovo file con un solo foglio).

---

## 🔐 Sicurezza: chi può modificare cosa?

- **Solo tu** (e le persone con accesso al repo) puoi caricare/modificare i file Excel su GitHub
- I **visitatori del sito** possono solo **vedere** le classifiche — non hanno alcun modo di modificare i dati ufficiali
- Un visitatore può, dal proprio browser, caricare un file Excel "in locale" per fare prove (es. simulare un risultato): questa operazione **resta solo sul suo dispositivo** e non influenza ciò che vedono gli altri visitatori. Sull'app questi file vengono marcati come "📁 Override locale".

---

## 🧪 Test prima di pubblicare (consigliato)

Prima di caricare un file su GitHub (operazione che lo rende immediatamente pubblico), puoi verificare che funzioni:

1. Apri il sito `https://fringuello79.github.io/atrs/` sul tuo dispositivo
2. Sulla scheda "Gare", trova la riga della distanza che ti interessa
3. Tocca "Carica Excel" e seleziona il file dal tuo dispositivo
4. Controlla che gli atleti siano caricati correttamente, vai sulla scheda "Classifica" e verifica i punteggi
5. Se tutto torna, **ora puoi caricarlo su GitHub** col nome corretto
6. Se invece ci sono problemi (colonne sbagliate, atleti mancanti, ecc.), correggi il file Excel e ripeti il test

> Il file caricato in locale è solo sul tuo browser, non viene visto da nessun altro. Per cancellarlo, tocca "Rimuovi" sulla riga della gara.

---

## 🆘 Risoluzione problemi

**"Ho caricato il file ma non lo vedo nell'app"**
- Controlla il nome: deve essere esattamente come in tabella, **lowercase, con il trattino, senza spazi**. Errori comuni: `Voltigno-19km.xlsx` (V maiuscola), `voltigno_19km.xlsx` (underscore al posto del trattino), `voltigno-19.xlsx` (manca "km").
- Controlla la cartella: il file deve essere in `classifiche/`, non nella root del repo.
- Aspetta 30 secondi e fai refresh forzato (`Ctrl+F5`).

**"Vedo errore al caricamento del file"**
- Apri il file in Excel: deve avere almeno le colonne "Family Name" / "Cognome" e "First Name" / "Nome".
- Se le colonne hanno nomi strani (es. "Cognome atleta"), rinominale semplicemente in "Cognome" e "Nome".
- Salva nel formato `.xlsx` standard (non `.xls` vecchio).

**"L'app non mostra le mie modifiche dopo l'upload su GitHub"**
- È quasi sempre un problema di cache. Fai refresh forzato sull'app (`Ctrl+F5` desktop, oppure tira giù la pagina sul mobile per ricaricare).
- Verifica che GitHub Pages sia attivo: `Settings → Pages → Source: Deploy from a branch → main`. La pubblicazione di un nuovo file impiega 1-2 minuti.

**"Voglio caricare un file con un nome diverso"**
- Non si può. I nomi sono fissi perché l'app sa esattamente quale file appartiene a quale gara. Se proprio devi conservare il nome originale del cronometraggio, fai una **copia** rinominata e carica quella su GitHub.

---

## 📝 Checklist veloce post-gara

Quando arrivano i risultati:

- [ ] Ricevuto file Excel dal cronometraggio
- [ ] (Opzionale) Verifica colonne: `Family Name`, `First Name`, `Gender`, `BirthDate`, `Team`
- [ ] Rinominato il file con il nome corretto della tabella
- [ ] Test in locale aprendo il sito e caricando il file dal dispositivo
- [ ] Punteggi e atleti verificati
- [ ] File caricato in `classifiche/` su GitHub
- [ ] Commit con messaggio descrittivo (es. "Aggiunta classifica Voltigno 19km")
- [ ] Verifica sul sito pubblico che la nuova gara appaia con badge "📡 Ufficiale"

---

*Ultima modifica: maggio 2026*
