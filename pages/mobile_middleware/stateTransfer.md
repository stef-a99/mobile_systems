# STATE TRANSFER

Pattern che consente la realizzazione dell'handoff tramite l'utilizzo di **rendez-vous points**.
Il **rendez-vous** è un pattern simmetrico per la sincronizzazione ,che **permette a due o più entità di sincronizzare le loro attività.**

Esempio:

![](Pasted%20image%2020240608191200.png)

I client A e B sono entità possibilmente mobili. Il punto di rendez-vous è un'entità fissa (o poco mobile) e nota a priori ai client.


##### S.T. & handoff

Il client che è connesso al vecchio AP e vuole connettersi ad uno nuovo, aggiorna il suo stato sul punto di rendez-vous e si connette al nuovo AP. Il correspondent node interagisce con il punto di rendez-vous per conoscere lo stato del client e poterci communicare.

![](Pasted%20image%2020240608191524.png)