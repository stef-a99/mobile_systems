# OBSERVER

Un *observer* si registra presso uno o più specifici *subject*, i quali notificano l'*observer* nel caso in cui subiscano modifiche. 

#### VANTAGGI
1) **decoupling tra subject e observer**
2) supporto alla **comunicazione di gruppo** (un *subject* può avere più *observer*)

#### SVANTAGGIO
1) Scalabilità limitata