# MODELLO RUNTIME


Di default, ogni applicazione è eseguita in una **Dalvik VM dedicata**, e all'interno di un proprio **processo separato**.
Ad ogni app è associato:
- **user ID**;
- **group ID**;
che sono selezionati da un intervallo definito a livello di sistema:

$$FIRST_{APPLICATION\ UID} - LAST_{APPLICATION\ UID}$$

I **permessi** sono stabiliti a seconda dello user ID e del group ID e possono esserne concessi di più specifici, andando a **dichiararli nel manifest**.