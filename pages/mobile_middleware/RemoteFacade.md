# REMOTE FACADE

Un dispositivo mobile effettua richieste ad un singolo **entry point**, detto *==facade==*, tramite un' **interfaccia coarse-grained**.
La *facade* comunica con diversi servizi esterni, implementati tramite **oggetti** (*fine-grained*) e restituisce dei risultati al client.

#### Vantaggi
1) decoupling tra Client e Server --> **comunicazione trasparente** agli occhi del client, che non conosce quali servizi o funzioni sono utilizzati per implementare le operazioni richieste.
2) il client può avere differenti protocolli di comunicazione, mentre il server agisce da **gateway remoto**, che trasforma le richieste del client nello standard usato dai servizi
3) semplice protocollo di *request/response* --> comunicazioni asincrone --> no problemi relativi alle disconnessioni.