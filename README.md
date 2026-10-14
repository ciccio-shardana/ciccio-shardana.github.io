# Personal Hub — Francesco Aymerich

> Hub centrale, portfolio e punto di accesso rapido per tutti i progetti, dispense, guide e siti web del workspace.

## 🚀 Apertura Rapida (Zero-Build & Doppio Click)
Questo progetto segue gli standard di workspace definiti in `AGENTS.md` e la skill `modern-web-ui`:
- **Nessuna dipendenza né build**: Apri direttamente `index.html` con un **doppio click** da Finder o da terminale:
  ```bash
  open /Users/boss/Documents/ANTI/PROGETTI/personal-hub/index.html
  ```

---

## 💎 Caratteristiche & Componenti

1. **Estetica Componentry Dark Minimal**:
   - Palette scura: `#09090b` (background zinc profondo), `#121215` (card di primo livello), bordi semi-trasparenti `rgba(255,255,255,0.08)`.
   - Tipografia: font `Geist` e `Geist Mono` con tracking compatto.
2. **Hero con Kinetic Text Reveal**:
   - Ingresso graduale scaglionato per il nome e i ruoli chiave.
3. **Flight Status Metrics**:
   - Scheda tecnica sintetica dello stato accademico, di ricerca e dei progetti del workspace.
4. **Vetrina Progetti (Orbit Card Grid)**:
   - Filtro istantaneo per categoria (*Tutti*, *Neurotech & Robotica*, *Strumenti & AI*, *Outdoor & Viaggi*).
   - Collegamento diretto a tutti i progetti presenti nel workspace:
     - `robotics-pitch`
     - `automazione-appunti`
     - `neuroengineering_course`
     - `antigravity-guide.html`
     - `VIAGGI/17-18 ottobre 2026 (Rifugio Riva)`
     - `VIAGGI/11-13 settembre 2026 (Langhe & Monferrato)`
5. **Timeline dei Siti Web Pubblicati (Release Radar)**:
   - Cronologia verticale dei siti e delle presentazioni web rilasciate nel tempo con date, tipo di progetto e link rapido.
6. **Curriculum Vitae & Stampa PDF Ottimizzata**:
   - Scheda CV professionale con focus su Ingegneria Biomedica, Neuroscienze computazionali e Machine Learning.
   - Pulsante dedicato **Scarica / Stampa CV (PDF)** che attiva la stampa browser con foglio A4 pre-formattato via `@media print`.
7. **Command Palette (`⌘K` o `Ctrl+K`)**:
   - Modal di ricerca universale istantanea navigabile con tastiera (frecce Su/Giù e Invio per aprire direttamente il progetto).
8. **Magnetic Dock Flottante**:
   - Barra di navigazione sul fondo dello schermo con effetto frosted glass e scrollspy attivo.
9. **Canali & Social**:
   - Card dedicate per GitHub, LinkedIn, Instagram ed Email.

---

## 🛠 Come Aggiungere Nuovi Progetti o Siti Web
Per aggiungere una nuova scheda progetto o un nuovo nodo nella timeline, apri `index.html`:
1. **Nella Griglia Progetti**: duplica una card `.project-card` nella sezione `#progetti`, aggiorna il percorso `href` e la categoria `data-category`.
2. **Nella Timeline**: aggiungi un blocco `.timeline-node` all'interno di `.timeline-wrapper` nella sezione `#timeline`.
3. **Nell'indice della Command Palette**: aggiungi il nuovo oggetto all'array `searchItems` nel tag `<script>`.
