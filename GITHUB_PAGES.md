# GitHub Pages Setup

Questo repository è configurato per utilizzare GitHub Pages con Jekyll per convertire automaticamente i file Markdown in pagine HTML.

## Come funziona

1. **File Markdown**: I file `.md` nelle cartelle `Demos/` e `Materiale/` vengono automaticamente convertiti in pagine HTML
2. **Jekyll Collections**: Il contenuto è organizzato in tre collezioni:
   - `_trainer_demos`: Demo per formatori
   - `_student_demos`: Demo per studenti  
   - `_materiale`: Materiale di supporto
3. **Layout automatico**: Ogni tipo di contenuto ha un layout specifico per la presentazione

## Struttura del sito

```
https://massimobonanni.github.io/Paestum-Tech-Days-2025/
├── index.html (Homepage principale)
├── trainer-demos/ (Lista demo formatori)
├── student-demos/ (Lista demo studenti)
├── materiale/ (Lista materiale)
└── [contenuti individuali]
```

## Aggiornamento del contenuto

### Automatico
Il sito viene aggiornato automaticamente quando:
- Si modifica un file `.md` nel branch `main`
- Si modificano i layout o la configurazione Jekyll

### Manuale
È possibile attivare manualmente l'aggiornamento:
1. Vai su GitHub → Actions
2. Seleziona "Deploy to GitHub Pages"
3. Clicca "Run workflow"

## Aggiungere nuovo contenuto

Per aggiungere nuovo contenuto:

1. **Demo per formatori**: Aggiungi file `.md` in `Demos/Trainer/`
2. **Demo per studenti**: Aggiungi file `.md` in `Demos/Student/`
3. **Materiale**: Aggiungi file `.md` in `Materiale/`

I file verranno automaticamente:
- Copiati nelle collezioni Jekyll appropriate
- Dotati di front matter per Jekyll
- Inclusi nella navigazione del sito

## Video e file multimediali

I file video (`.mp4`) vengono copiati insieme ai markdown e mantengono i riferimenti relativi, quindi funzioneranno correttamente nelle pagine HTML.

## Personalizzazione

- **Layout**: Modifica i file in `_layouts/`
- **Stili**: Aggiungi CSS personalizzato nei layout
- **Configurazione**: Modifica `_config.yml`
- **Homepage**: Modifica `index.html`