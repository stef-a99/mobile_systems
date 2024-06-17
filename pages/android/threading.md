# THREADING

Android segue il ***single thread model***, in cui ogni app è associata ad un singolo thread, che esegue tutte le Activity che la compongono.
Ogni thread è dotato di un *loop infinito*, per gestire localmente la coda dei messaggi: riceve eventi esterni (di sistema/input dall'utente), che possono essere inviati alle activity.

![](Pasted%20image%2020240610110118.png)