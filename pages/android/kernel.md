# KERNEL LAYER

Basato su Linux 3.x e unito ad un Hardware Abstraction Layer (HAL).
Non è un kernel vero e proprio, perché mancano:
- **gestione delle finestre nativo**;
- supporto alla libreria **GNU C**;
- **utility standard** di Linusio (come la CLI).
Infatti, non possiamo creare manualmente dei processi e non possiamo gestire le finestre come nei normali sistemi popitivi.

Tuttavia, sono presenti alcune estensioni:
- **Gestore di memoria condivisa - ASHMEM**, che consente la comunicazione tra processi appartenenti ad applicazioni diverse tramite **memoria condivisa**. Si ha anche il **conteggio dei riferimenti** e la **deallocazione automatica** da parte del kernel.
- **IPC Binder**, che fornisce dei servizi di sistema attraverso cui un'applicazione Android può accedere alle risorse di sistema o all'HW sottostante, tramite l'impiego di Ashmem.
- **Gestione avanzata del consumo di energia**, tramite i [**Wakelocks**](wakelock.md).