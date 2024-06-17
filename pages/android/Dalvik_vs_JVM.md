# Classic Java vs Android-Java

# DALVIK VM

La Dalvik VM è *registry-based*, ovvero sfrutta l'architettura ARM, a differenza della JVM tradizionale, che è stack-based (dove i dati sono manipolati tramite push/pop verso/da uno stack).

- ###### Stack-based vs Registry-based
  
  Le prime hanno una maggiore portabilità, mentre le seconde sono più performanti in termini di velocità di esecuzione e consumo di risorse.

La Dalvik VM interpreta ed esegue i file **dex**, ottenuti con la **trasformazione dei file di classe**, per ridurre del 30% le istruzioni necessarie e migliorare le performance a runtime (dex non è compatibile col Java ordinario, poiché prevede meno istruzioni). Infine, fornisce supporto alla *garbage collection*.
Da Android Lollipop è stata sostituita da ART.