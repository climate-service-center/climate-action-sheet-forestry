Indizes für Beobachtungsdaten und Ergebnisse der EURO-CORDEX Simulationen für verschiedene globale Erwärmungsstufen
-------------------------------------------------------------------------------------------------------------------

Jede in Tabelle 3 dargestellte Klimakenngröße wurde mit einer Experteneinschätzung ergänzt, die die Belastbarkeit der Ergebnisse beschreibt. Dies ist durch die unterschiedlichen Grautöne in der Tabelle gekennzeichnet: “je dunkler das Grau, um so eindeutiger die Klimaänderung“. Wenn eine Mehrzahl der Ergebnisse der Klimamodelle für eine Kenngröße eine statistisch signifikante Zunahme oder Abnahme zeigt, wird die Änderung im Folgenden als „robust“ bezeichnet (dunkelgrau). Wenn die Mehrzahl der Ergebnisse der Modelle keine deutlichen Änderungen, aber eine eindeutige Richtung der Änderungen angibt, ist eine „Tendenz zur Zu- bzw. Abnahme“ vorhanden (grau). Wenn die Ergebnisse der Klimamodelle etwa zu gleichen Teilen sowohl eine Zunahme als auch eine Abnahme zeigen, gibt es keine eindeutige Änderung (hellgrau/unklar). Unterhalb des Medians der Ergebnisse aller Klimasimulationen (hier fett und groß) befindet sich eine Angabe zur Bandbreite der möglichen Entwicklungen in Form einer minimalen und maximalen Änderung.

.. image:: plots/Karlsruhe_table_GWL_08212_08215_07334_Region_um_Karlsruhe_median_grey_300.png

In **Tabelle 3** sind die ausgewählten Klimakenngrößen und deren zukünftige mittlere Veränderungen im Vergleich zum Zeitraum 1971 bis 2000 jeweils für den Fall einer Erhöhung der globalen Mitteltemperatur um 1,5°C, 2°C, 3°C und 4°C im Vergleich zum vorindustriellen Niveau aufgelistet. In der 1. Spalte steht der mittlere beobachtete Wert über die Jahre von 1971 bis 2000 (E-OBS_). Die Klimaänderungen wurden mit einer Vielzahl von Modellen berechnet, deren Ergebnisse zwischen dem angegebenen Minimum und Maximum (Min-Max) liegen. Darüber steht die Zahl (Median), unter und über der jeweils die Hälfte der Modelle liegen.

Diese Tabelle kann mit dem folgenden Notebook erstellt werden:


.. code-block:: console

   $ Notebooks/INDICES-TABLE/read_csv_cordex_GWL-MEDIAN-MIN-MAX-all-bw.ipynb


Das Notebook verwendet die Daten die in folgendem Verzeichnis liegen:

.. code-block:: console

   $ input_data


.. _E-OBS: https://cds.climate.copernicus.eu/cdsapp#!/dataset/insitu-gridded-observations-europe
