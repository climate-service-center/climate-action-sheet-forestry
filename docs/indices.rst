Klimaparameter
--------------

Die verwendeten Klimaparamter werden mit dem `index_calculator`_ berechnet. Der *Index Calculator* verwendet xclim_.

+-------+--------------------------------+--------------------------+---------+
| Index | Name                           | Variable                 | Ausgabe |
+=======+================================+==========================+=========+
|  TG   | Mittlere Temperatur            | Temperatur               | Jahr    |
+-------+--------------------------------+--------------------------+---------+
|  FD   | Anzahl der Frosttage           | Minimumtemperatur < 0°C  | Jahr    |
+-------+--------------------------------+--------------------------+---------+
|  LFD  | Anzahl der Spätfrosttage       | Minimumtemperatur < 0°C  | Jahr    |
+-------+--------------------------------+--------------------------+---------+
|       | zwischen April und Juni        |                          |         |
+-------+--------------------------------+--------------------------+---------+
|  SU30 | Anzahl der Hitzetage           | Maximumtemperatur > 30°C | Jahr    |
+-------+--------------------------------+--------------------------+---------+
|  SU35 | Anzahl der Hitzetage           | Maximumtemperatur > 35°C | Jahr    |
+-------+--------------------------------+--------------------------+---------+
|  RRm  | mittlerer Tagesniederschlag    | Niederschlag             | Jahr    |
+-------+--------------------------------+--------------------------+---------+
|       |                                |                          | Saison  |
+-------+--------------------------------+--------------------------+---------+
|  DD   | Anzahl der Trockentage         | Niederschlag < 1mm/day   | Jahr    |
+-------+--------------------------------+--------------------------+---------+
|       |                                |                          | Saison  | 
+-------+--------------------------------+--------------------------+---------+
|  DSx  | Max. Länge der Trockenperioden | Niederschlag             | Jahr    |
+-------+--------------------------------+--------------------------+---------+
|       | Länge >= 5 Tage                |                          |         |
+-------+--------------------------------+--------------------------+---------+
|  DSf  | Anzahl der Trockenperioden     | Niederschlag             | Jahr    |
+-------+--------------------------------+--------------------------+---------+
|       | Länge >= 5 Tage                |                          |         |
+-------+--------------------------------+--------------------------+---------+
|  HSx  | Max. Länge der Hitzeperioden   | Maximumtemperatur >30°C  | Jahr    |
+-------+--------------------------------+--------------------------+---------+
|       | Länge >= 3 Tage                |                          |         |
+-------+--------------------------------+--------------------------+---------+
|  HSf  | Anzahl der Hitzeperioden       | Maximumtemperatur >30°C  | Jahr    |
+-------+--------------------------------+--------------------------+---------+
|       | Länge >= 3 Tage                |                          |         |
+-------+--------------------------------+--------------------------+---------+

Die in **Tabelle 2** aufgeführten Klimaparameter werden auf Grundlage der Ergebnisse der EURO-CORDEX Simulationen berechnet.




.. _`index_calculator`: https://github.com/climate-service-center/index_calculator

.. _xclim: https://github.com/Ouranosinc/xclim
