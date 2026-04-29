Perché questo ora "funziona":
Fallback Download: Se clicchi "Salva" e il tuo browser non ti permette di sovrascrivere il file esistente (magari perché non sei su un sito HTTPS sicuro), 
l'app scaricherà semplicemente un nuovo file JSON. Non avrai l'errore "non funziona", avrai un download.

Gestione Eccezioni: Ho aggiunto dei blocchi try/catch che impediscono all'app di bloccarsi se l'utente chiude la finestra di dialogo del file.

UI Pulita: I pulsanti sono chiaramente distinti tra "Carica" (per riprendere il lavoro) e "Salva" (per memorizzarlo).

Nota importante: Per usare la funzione di sovrascrittura dello stesso file, devi eseguire questa pagina web tramite un piccolo server locale o caricarla online 
(GitHub Pages, Netlify, ecc.). Se apri il file .html direttamente col doppio clic dal desktop, il browser spesso blocca la scrittura dei file per sicurezza e userà il download classico.
################################################################
29/04/2026
Ho integrato il Pad per la firma digitale, la logica di reset automatico al cambio mese con scollegamento del file, e ho rifinito il layout del PDF per includere la firma acquisita.

Ho anche aggiunto la libreria signature_pad nell'head.
