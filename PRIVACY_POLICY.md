# Privacy Policy — NobumangaDownloader

**Sviluppatore:** Nobuscimmia  
**Ultimo aggiornamento:** Giugno 2025  
**Versione app:** 1.0.0

---

## 1. Raccolta dati

NobumangaDownloader **NON raccoglie né trasmette dati personali** degli utenti.

Tutti i dati generati dall'app (libreria manga, impostazioni, cronologia download) sono salvati **esclusivamente sul dispositivo dell'utente** in un database SQLite locale:

```
C:\Users\[utente]\AppData\Roaming\NobumangaDownloader\library.db
```

Nessun dato viene mai inviato a server esterni, analizzato o condiviso con terze parti.

---

## 2. Connessioni di rete

L'app si connette a internet **solo su richiesta esplicita dell'utente** per:

| Destinazione | Scopo | Quando |
|---|---|---|
| `mangaworld.mx` | Scaricare i manga selezionati dall'utente | Solo durante la ricerca o il download |
| `raw.githubusercontent.com` | Controllare se esiste una nuova versione dell'app | All'avvio dell'app (una volta) |

Nessun'altra connessione di rete viene effettuata.

---

## 3. Cookie e tracciamento

L'app **non utilizza**:
- Cookie di alcun tipo
- Tracker comportamentali
- Strumenti di analytics (Google Analytics, Mixpanel, ecc.)
- Advertising SDK
- Fingerprinting del dispositivo

---

## 4. Contenuti di terze parti

I manga scaricati tramite l'app provengono da **mangaworld.mx**, un sito di terze parti.  
Nobuscimmia non è affiliato con mangaworld.mx e non è responsabile dei contenuti presenti sul sito.

L'utente è responsabile del rispetto dei termini di servizio di mangaworld.mx e delle leggi sul copyright applicabili nel proprio paese.

---

## 5. Dati salvati localmente

L'app salva in locale esclusivamente:

- **Libreria manga**: titoli, URL, copertine, capitoli aggiunti dall'utente
- **Impostazioni**: cartella di download, formato preferito, orario scheduler
- **Log di sistema**: file `nobumanga.log` per debug tecnico, non contiene dati personali

L'utente può cancellare tutti i dati in qualsiasi momento eliminando la cartella:
```
C:\Users\[utente]\AppData\Roaming\NobumangaDownloader\
```

---

## 6. Sicurezza

- Tutti i dati locali sono accessibili solo dall'utente proprietario del dispositivo
- Non vengono effettuati backup automatici su cloud
- Il codice sorgente è disponibile su GitHub per verifica pubblica

---

## 7. Minori

L'app non è destinata a utenti di età inferiore ai 13 anni.  
Non raccogliamo consapevolmente dati da minori.

---

## 8. Modifiche a questa policy

Eventuali modifiche saranno pubblicate nella pagina GitHub del progetto con data aggiornata.  
L'uso continuato dell'app dopo le modifiche costituisce accettazione della nuova policy.

---

## 9. Contatti

Per domande sulla privacy:  
📧 **nobuscimmia@gmail.com**  
🌐 **github.com/nobuscimmia/nobumanga-downloader**
