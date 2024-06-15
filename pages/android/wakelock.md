# WAKELOCKS

I *wakelocks* sono dei lock che permettono alle applicazioni di accedere alle funzioni del Power Manager, così che ogni applicazione può controllare il consumo energetico applicando le proprie policy.

I wakelocks sono un esempio di [**cross-layering pattern**](crossLayering.md), poiché il livello applicativo può interagire direttamente coi livelli HW sottostanti.

Il lock è rilasciato quando l'applicazione non è più (quando la metto in pausa o la chiudo).
![](Pasted%20image%2020240610092229.png)