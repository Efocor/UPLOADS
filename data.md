Kutral cuenta con un total de 1792 núcleos funcionando a 2.6 GHz, 1096 TB de almacenamiento y 13 TB de RAM, todo interconectado mediante InfiniBand a 40 G/s. El cluster esta compuesto por 4 tipos de equipos

    Nodos de computo: Utilizados para cálculos en general

IBM DX360 m2
55 nodos en total
16 CPUs Intel Xeon X5550 2.67 GHz
60 a 128 GB RAM
250 GB de disco duro
Conexión infiniband

Equipo computo.png

    Nodos storage: Utilizados para el almacenamiento de todo el sistema

HP ProLiant DL380p Gen8
11 nodos en total
24 CPUs Intel Xeon CPU E5-2630 2.30 GHz
220 GB RAM
12 discos duros de 8TB (3 de respaldo)
Conexión infiniband

Nodo storage.png

    Nodos memoria: Utilizados principalmente para cálculos area genómica

Dell PowerEdge R630 
5 nodos en total
72 CPUs Intel Xeon CPU E5-2695 2.10 GHz
1 TB RAM
600 GB disco duro
Conexión infiniband 

Nodo memoria.png

    Nodos gpu: Utilizados para machine learning

Equipo V100
112 CPUs Intel Xeon Gold 6238R 2.20 GHz
3 GPUs Tesla V100S-PCI 32 GB HBM2 5120 cores
1 TB RAM
18 TB HDD

Equipo A100
64 CPUs AMD EPYC 7313 3.00 GHz
2 GPUs A100 SXM4 40 GB HBM2 6912 cores
2 GPUs
315 GB RAM
4 TB HDD

Equipo P40
88 CPUs Intel Xeon E5-2699 2.20 GHz
2 GPUs Tesla P40 24 GB GDDR5 3840 cores
500 GB RAM
400 GB HDD

-------------------------------------------------------------

(pathonet) [fcorrea@toki-hm-4 PathoNet]$ gnodes

+- ngen-ko - 16 cores & 41GB ----+
| host54   42G  ................ |
+--------------------------------+

+- ngen-ko - 16 cores & 50GB ----+
| host58   51G  ................ |
+--------------------------------+

+- ngen-ko - 16 cores & 54GB ----+--------------------------------+
| host45   55G  ................ | host47   55G  ................ |
+--------------------------------+--------------------------------+

+- ngen-ko - 16 cores & 58GB ----+
| host37   59G  ................ |
+--------------------------------+

+- ngen-ko - 16 cores & 61GB ----+--------------------------------+--------------------------------+--------------------------------+
| host17   38G  .._____________O | host40   62G  ................ | host48   62G  ................ | host57   62G  ................ |
| host36   62G  ................ | host41   62G  ................ | host49   62G  ................ |                                |
| host38   62G        DOWN       | host44   62G  ................ | host53   62G  ................ |                                |
| host39   62G  ................ | host46   62G  ................ | host55   62G        DOWN       |                                |
+--------------------------------+--------------------------------+--------------------------------+--------------------------------+

+- ngen-ko - 16 cores & 78GB ----+
| host15   78G        DOWN       |
+--------------------------------+

+- ngen-ko - 16 cores & 86GB ----+
| host02   86G        DOWN       |
+--------------------------------+

+- ngen-ko - 16 cores & 101GB ---+--------------------------------+--------------------------------+--------------------------------+
| host03  102G  ................ | host18  102G        DOWN       | host30  102G        DOWN       | host34  102G        DOWN       |
| host16    0G  ________OOOOOOOO | host25  102G        DOWN       | host32  102G        DOWN       |                                |
+--------------------------------+--------------------------------+--------------------------------+--------------------------------+

+- ngen-ko - 16 cores & 109GB ---+
| host22  109G        DOWN       |
+--------------------------------+

+- ngen-ko - 16 cores & 117GB ---+--------------------------------+
| host06  117G  ................ | host12  117G  ................ |
+--------------------------------+--------------------------------+

+- ngen-ko - 16 cores & 125GB ---+--------------------------------+--------------------------------+--------------------------------+
| host01  125G  ................ | host10  125G  ................ | host19  125G        DOWN       | host27  125G        DOWN       |
| host04  125G  ................ | host11  125G        DOWN       | host21  125G  ................ | host28  125G        DOWN       |
| host05  125G  ................ | host13  125G  ................ | host24  125G        DOWN       | host29  125G        DOWN       |
| host08  125G  ................ | host14  125G  ................ | host26  125G        DOWN       |                                |
+--------------------------------+--------------------------------+--------------------------------+--------------------------------+

+- ngen-ko - 24 cores & 187GB -----------+
| SRV03   188G  ........................ |
+----------------------------------------+

+- ngen-ko - 64 cores & 313GB & 1 GPUs ----------------------------------------------+
| tokikura  249G  ........................................................________ * |
+------------------------------------------------------------------------------------+

+- ngen-ko - 72 cores & 1006GB -------------------------------------------------------------+
| toki-hm-1  943G  ........................................................OOOOOOOOOOOOOOOO |
| toki-hm-2 1007G  ........................................................................ |
| toki-hm-3  907G  .............................................................._________O |
+-------------------------------------------------------------------------------------------+

+- ngen-ko - 88 cores & 502GB & 2 GPUs ---------------------------------------------------------------------+
| wuruwe  493G  ......................................................................................__ ** |
+-----------------------------------------------------------------------------------------------------------+

+- ngen-ko - 88 cores & 1006GB --------------------------------------------------------------------------+
| dungu   607G  ......................................_________________OOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOOO |
+--------------------------------------------------------------------------------------------------------+

+- ngen-ko - 112 cores & 1006GB & 3 GPUs --------------------------------------------------------------------------------------------+
| v100   1007G  ................................................................................................................ *** |
+------------------------------------------------------------------------------------------------------------------------------------+
