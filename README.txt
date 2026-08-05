ACF Fiorentina - Set Pieces App PWA v117

COME USARLA SU IPAD
1. Carica l'intera cartella su un hosting HTTPS.
2. Apri in Safari l'indirizzo che termina con /index.html.
3. Tocca Condividi.
4. Tocca "Aggiungi alla schermata Home".
5. Apri l'app dalla nuova icona.
6. Dopo la prima apertura online, l'app potrà essere usata offline.

IMPORTANTE
- Non aprire index.html direttamente dall'app File o da Quick Look.
- Service worker e installazione PWA funzionano soltanto tramite HTTPS oppure localhost.
- Backup e importazione restano locali sul dispositivo.
- Le funzioni PNG/PDF dipendono dalle librerie esterne già richiamate nell'HTML:
  apri almeno una volta l'app con connessione prima di usarle offline.


NOVITÀ v117
- Barra touch sotto il campo
- Copia, incolla ed elimina
- Allineamento orizzontale e verticale
- Distribuzione uniforme
- Gestione livelli per oggetti grafici
- Blocco modifiche
- Modalità campo intero


NOVITÀ v117 - BACKUP UNIVERSALE
- Nuovo formato .acf compatibile con Mac, iPad, Safari e Chrome
- Importazione di .acf, .setpieces, .acfbackup, .json e .txt
- Compatibilità con tutti i backup precedenti
- Lettura UTF-8 robusta tramite ArrayBuffer
- Supporto ai file rinominati o salvati tramite AirDrop/iCloud
- Esportazione tramite pannello Condividi nativo su iPad
- Controllo e riparazione automatica dei dati importati
- Messaggi di errore dettagliati


NOVITÀ v117
- Pulsante Torna indietro, equivalente a Command+Z
- Allinea H rinominato in Orizzontale
- Allinea V rinominato in Verticale


CORREZIONE v129 - POSIZIONI INVARIATE
- Rapporto del campo fissato a 1000 × 620 su Mac, iPad e fullscreen
- Nessuna deformazione passando tra dispositivi
- Nessun riallargamento entrando in modalità Campo intero
- Coordinate di giocatori, frecce, forme, palloni e testi mantenute in percentuale


NOVITÀ v129
- Dimensione predefinita delle maglie: 90%
- Trascinamento più fluido di pallone e testi
- Stessa anagrafica completa per Fiorentina e avversari
- Cursore Tratteggio per frecce dritte e curve
- Punta delle frecce sempre piena
- Controllo completo della sintassi JavaScript


NOVITÀ v129
- Nuovo sfondo del campo basato sull'immagine campo.png
- Vecchie linee CSS del campo disattivate
- Coordinate e posizioni degli oggetti mantenute invariate
- Compatibilità Mac, iPad, fullscreen, PNG e PDF


NOVITÀ v129
- Movimento pallone più fluido su Mac e iPad
- Movimento testo più fluido su Mac e iPad
- Eliminati i rerender durante il trascinamento
- Pointer capture e requestAnimationFrame per un drag stabile
- Bloccato lo scorrimento involontario della pagina durante il drag


NOVITÀ v129
- Flag Numero nel cerchio per Fiorentina e avversari
- Opzione Avversari: linea tratteggiata da compilare a penna
- Navigazione schema precedente/successivo in Campo intero
- Tratteggio delle frecce corretto
- Punta delle frecce sempre piena
- Nuove preferenze incluse nel backup


NOVITÀ v129
- Linea avversari continua anziché tratteggiata
- Linea avversari spostata più in basso
- Flag numero applicato soltanto ai giocatori selezionati
- Possibilità di mostrare/nascondere il numero per gruppi diversi
- Stato misto del flag quando la selezione contiene giocatori con impostazioni differenti


NOVITÀ v129
- Flag Linea nei selezionati applicato soltanto agli avversari selezionati
- Possibilità di mostrare o nascondere la linea per singoli avversari o gruppi
- Stato intermedio del flag per selezioni miste
- Il flag resta disabilitato se non è selezionato alcun avversario


FIX v129 - TRATTEGGIO FRECCE
- Applicato realmente stroke-dasharray al corpo di frecce dritte e curve
- Punta della freccia sempre piena
- Quattro livelli: continua, tratto corto, tratto medio, puntinata
- Aggiornamento immediato del cursore anche su iPad
- Valore salvato nei progetti e nei backup
- Compatibilità con frecce create nelle versioni precedenti


NOVITÀ v129 - AGGIORNAMENTO AUTOMATICO PWA
- Cache service worker versionata per ogni release
- Eliminazione automatica delle cache precedenti
- index.html sempre controllato dalla rete prima della cache
- Asset aggiornati in background con stale-while-revalidate
- Controllo aggiornamenti all'avvio, al ritorno in primo piano e ogni 5 minuti
- Attivazione automatica della nuova versione
- Salvataggio dello stato prima del refresh invisibile
- Nessuna necessità di svuotare manualmente la cache


NOVITÀ v129 - RENDERING CAMPO
- Canvas logico fisso 1000 × 620
- Il campo viene ridimensionato soltanto tramite transform: scale()
- Maglie, palloni, testi, frecce e forme crescono insieme al campo
- Nessun oggetto resta piccolo entrando in Campo intero
- Coordinate identiche tra Mac, iPad e fullscreen
- Adattamento automatico a rotazione e ridimensionamento


FIX v129 - CAMPO INTERO
- Corretto il campo ingrandito e tagliato in modalità fullscreen
- Eliminata la centratura tramite translate, instabile su Safari e Chrome
- Posizione del canvas calcolata esplicitamente in pixel
- Scala uniforme per campo, maglie, palloni, testi, frecce e forme
- Campo sempre centrato e interamente visibile
- Ricalcolo automatico dopo rotazione e cambio dimensione
