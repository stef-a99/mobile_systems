# MODELLO RUNTIME


Di default, ogni applicazione è eseguita in una **Dalvik VM dedicata**, e all'interno di un proprio **processo separato**. **Maggiore sicurezza**, perché app isolate e no visibilità reciproca MA **maggior consumo di risorse**.
Ad ogni app è associato:
- **user ID**;
- **group ID**;
che sono selezionati da un intervallo definito a livello di sistema:

$$FIRST_{APPLICATION\ UID} - LAST_{APPLICATION\ UID}$$

I **permessi** sono stabiliti a seconda dello user ID e del group ID e possono esserne concessi di più specifici, andando a **dichiararli nel manifest**.
Inoltre, è possibile **chiedere all'utente** di dare permessi aggiuntivi a runtime. Esempio: aggiornamento dell'app. In questo caso si possono aggiungere feature che richiedono permessi non esplicitati nel manifest; quindi chiedendoli all'utente a runtime si possono garantire.

In alternativa, si possono eseguire **diverse app in una singola Dalvik VM**: specifico nel manifest uno `sharedUserID`, condiviso da più applicazioni. Questo **ottimizza l'utilizzo delle risorse di sistema**, ma crea un **unico processo pesante** e comporta **potenziali problemi di sicurezza**, poiché le app avranno visibilità completa l'una dell'altra.