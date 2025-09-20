📐 Calcolo Raggio Centro Gola

Un’applicazione web interattiva sviluppata in HTML, CSS, JavaScript e Bootstrap, pensata per calcolare rapidamente il Centro Gola di un anello (interno o esterno) e tenere traccia dei calcoli effettuati.

🚀 Funzionalità principali

Calcolo del Centro Gola
Inserisci:

Tipo di anello (IR interno o AR esterno)

Fondo pista (mm)

Due valori del raggio sfera
L’app calcola il centro gola e lo mostra con tre decimali di precisione.

Storico dei calcoli

Salvataggio automatico di ogni calcolo in LocalStorage

Storico consultabile con data/ora e dettagli

Possibilità di eliminare singoli calcoli o cancellare tutto

Operazioni sui valori salvati

Seleziona due calcoli dallo storico e somma/sottrai i loro valori

Salva il risultato come nuovo calcolo con nota

Interfaccia user-friendly

Design responsive con Bootstrap 5

Icone intuitive con Bootstrap Icons

Popup interattivi con SweetAlert2

🖼️ Anteprima interfaccia

Schermata principale con selettori e input per il calcolo

Storico calcoli sulla destra con possibilità di operare sui valori salvati

Notifiche popup per errori, conferme e risultati

🛠️ Tecnologie usate

HTML5 per la struttura

Bootstrap 5 per lo stile e il layout responsive

Bootstrap Icons per le icone

SweetAlert2 per i popup di notifica

JavaScript vanilla per la logica di calcolo e la gestione dello storico

📄 Struttura del codice

HTML
Contiene la struttura della pagina, i form di input, i pulsanti e i contenitori dello storico.

CSS
Utilizza principalmente Bootstrap, con poche regole personalizzate per lo stile di storico e pulsanti.

JavaScript

calcolaCentroGola(): esegue il calcolo principale

aggiornaStorico() / aggiornaSelectValori(): aggiorna lo storico e le opzioni dei <select>

eseguiOperazione(): esegue addizione o sottrazione tra due valori salvati

Funzioni per azzerare campi, cancellare lo storico e mostrare popup di informazioni

🧩 Requisiti

Browser moderno (Chrome, Edge, Firefox, Safari)

Connessione Internet (per caricare Bootstrap e SweetAlert2 da CDN)

▶️ Utilizzo

Apri il file centro_gola_improved.html in un browser.

Inserisci i valori richiesti.

Clicca Calcola per ottenere il risultato.

Consulta lo storico a destra per vedere i calcoli passati.

Usa i menu a tendina per fare operazioni tra valori salvati.

🔒 Persistenza dei dati

I calcoli sono salvati in LocalStorage, quindi rimangono disponibili finché non vengono eliminati manualmente o finché non si svuota la cache del browser.
