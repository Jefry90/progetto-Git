# 📐 Calcolo Raggio Centro Gola

Un'applicazione **web interattiva** sviluppata in HTML, CSS, JavaScript e Bootstrap, pensata per calcolare rapidamente il **Centro Gola** di un anello (interno o esterno) e tenere traccia dei calcoli effettuati.

## 🚀 Funzionalità Principali

### Calcolo del Centro Gola
- **Input richiesti:**
  - Tipo di anello (`IR` interno o `AR` esterno)
  - Fondo pista (mm)
  - Due valori del raggio sfera
- **Output:** Centro gola calcolato con precisione a tre decimali

### Storico dei Calcoli
- ✅ Salvataggio automatico in **LocalStorage**
- ✅ Consultazione storico con data/ora e dettagli completi
- ✅ Eliminazione singoli calcoli o cancellazione completa
- ✅ Persistenza dei dati tra le sessioni

### Operazioni sui Valori Salvati
- ➕ Addizione tra due calcoli dello storico
- ➖ Sottrazione tra due calcoli dello storico
- 💾 Salvataggio del risultato come nuovo calcolo con nota

### Interfaccia User-Friendly
- 📱 Design responsive con **Bootstrap 5**
- 🎨 Icone intuitive con **Bootstrap Icons**
- 🔔 Popup interattivi con **SweetAlert2**
- ⚡ Navigazione fluida e intuitiva

## 🖼️ Anteprima Interfaccia

- **Schermata principale** con selettori e input per il calcolo
- **Storico calcoli** laterale con operazioni sui valori salvati
- **Notifiche popup** per errori, conferme e risultati

## 🛠️ Tecnologie Utilizzate

| Tecnologia | Versione | Utilizzo |
|------------|----------|----------|
| **HTML5** | - | Struttura della pagina |
| **Bootstrap** | 5.x | Layout responsive e componenti UI |
| **Bootstrap Icons** | Latest | Iconografia |
| **SweetAlert2** | Latest | Sistema di notifiche |
| **JavaScript** | Vanilla ES6+ | Logica applicativa e gestione dati |

## 📁 Struttura del Codice

```
centro_gola_improved.html
├── HTML Structure
│   ├── Form di input
│   ├── Pulsanti di controllo
│   └── Container storico calcoli
├── CSS Styling
│   ├── Bootstrap 5 (CDN)
│   └── Stili personalizzati
└── JavaScript Logic
    ├── calcolaCentroGola()      # Calcolo principale
    ├── aggiornaStorico()        # Gestione storico
    ├── aggiornaSelectValori()   # Aggiornamento select
    ├── eseguiOperazione()       # Operazioni tra valori
    └── Utility functions        # Funzioni di supporto
```

## 🧩 Requisiti di Sistema

- **Browser moderno** (Chrome 90+, Edge 90+, Firefox 88+, Safari 14+)
- **Connessione Internet** (per CDN Bootstrap e SweetAlert2)
- **LocalStorage abilitato** (per persistenza dati)

## ▶️ Guida all'Utilizzo

### 1. Avvio dell'Applicazione
```bash
# Apri il file direttamente nel browser
open centro_gola_improved.html
```

### 2. Esecuzione di un Calcolo
1. Seleziona il **tipo di anello** (IR/AR)
2. Inserisci il **fondo pista** in millimetri
3. Inserisci i **due valori del raggio sfera**
4. Clicca **"Calcola"** per ottenere il risultato
5. Il calcolo viene automaticamente salvato nello storico

### 3. Gestione dello Storico
- **Visualizzazione:** I calcoli appaiono automaticamente nella sezione destra
- **Eliminazione singola:** Clicca sull'icona 🗑️ accanto al calcolo
- **Cancellazione completa:** Usa il pulsante "Cancella Storico"

### 4. Operazioni tra Valori
1. Seleziona **due calcoli** dai menu a tendina
2. Scegli l'**operazione** (+ o -)
3. Clicca **"Esegui Operazione"**
4. Il risultato viene salvato automaticamente con nota descrittiva

## 🔒 Persistenza dei Dati

I calcoli sono memorizzati nel **LocalStorage** del browser, garantendo:
- ✅ Disponibilità tra sessioni diverse
- ✅ Accesso offline ai dati salvati
- ⚠️ Perdita dati solo con svuotamento cache o eliminazione manuale
