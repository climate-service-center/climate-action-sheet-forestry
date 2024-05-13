Klimaparameter
--------------

Die verwendeten Klimaparamter werden mit dem `index_calculator`_ berechnet. Der *Index Calculator* verwendet xclim_.

+-------+--------------------------------+---------------+--------------+-----------------+
| Index | Name                           | Variable      | Ausgabe      | Kommentar       |
+=======+================================+===============+==============+=================+
|  TG   | Mittlere Temperatur            | tas           | Jahr         |                 |
+-------+--------------------------------+---------------+--------------+-----------------+
|  FD   | Anzahl der Frosttage           | tasmin< 0°C   | Jahr         |                 |
+-------+--------------------------------+---------------+--------------+-----------------+
|  LFD  | Anzahl der Spätfrosttage       | tasmin < 0°C  | Jahr         | April bis Juni  |
+-------+--------------------------------+---------------+--------------+-----------------+
|  SU30 | Anzahl der Hitzetage           | tasmax > 30°C | Jahr         |                 |
+-------+--------------------------------+---------------+--------------+-----------------+
|  SU35 | Anzahl der Hitzetage           | tasmax > 35°C | Jahr         |                 |
+-------+--------------------------------+---------------+--------------+-----------------+
|  RRm  | mittlerer Tagesniederschlag    | pr            | Jahr, Saison |                 |
+-------+--------------------------------+---------------+--------------+-----------------+
|  DD   | Anzahl der Trockentage         | pr < 1mm/day  | Jahr, Saison |                 |
+-------+--------------------------------+---------------+--------------+-----------------+
|  DSx  | Max. Länge der Trockenperioden | pr            | Jahr         | Länge >= 5 Tage |
+-------+--------------------------------+---------------+--------------+-----------------+
|  DSf  | Anzahl der Trockenperioden     | pr            | Jahr         | Länge >= 5 Tage |
+-------+--------------------------------+---------------+--------------+----------+------+
|  HSx  | Max. Länge der Hitzeperioden   | tasmax >30°C  | Jahr         | Länge >= 3 Tage |
+-------+--------------------------------+---------------+--------------+-----------------+
|  HSf  | Anzahl der Hitzeperioden       | tasmax >30°C  | Jahr         | Länge >= 3 Tage |
+-------+--------------------------------+---------------+--------------+-----------------+

Die in **Tabelle 2** aufgeführten Klimaparameter werden auf Grundlage der EURO-CORDEX Simulationen berechnet.



.. _`index_calculator`: https://github.com/climate-service-center/index_calculator

.. _xclim: https://github.com/Ouranosinc/xclim
