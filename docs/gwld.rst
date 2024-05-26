Globale Erwärmungsstufen
------------------------

Die Zeiträume, in denen die globalen Erwärmungsstufen (engl.: global warming level (GWL) `Nikulin (2018)`_) von +1.5, +2, +3 und +4 °C erreicht werden, beziehen sich auf den vorindustriellen Durchschnittswert der Jahre 1850 bis 1900. Dies bedeutet, dass der globale Mittelwert der bodennahen Temperatur um 1,5°C, 2°C, 3°C und 4 °C wärmer ist als im vorindustriellen Mittel. Die globalen Erwärmungsstufen werden für die globalen Projektionen von CMIP5 (*Coupled Modelling Intercomparison Project 5*) unter Verwendung eines gleitenden 30-Jährigen Mittelwertes berechnet.

Für die Berechnung der GWL wird die Methode aus dem `IPCC Atlas`_ verwendet (`Mathias Hauser`_). Für die hier vorliegenden Untersuchungen wurde lediglich die 20-Jährige Zeitspanne im Programm scripts/getGWL.R auf eine 30-Jährige Zeitspanne erweitert. Der `Unterschied`_ zwischen den Ergebnisse für eine 20-Jährige und 30-Jährige Zeitspanne ist gering, in Einzelfällen verschiebt sich das zentrale Jahr des gemittelten Zeitraumes um ein Jahr.

Vorindustriell und heute
........................

Die GWL werden im Vergleich zur vorindustriellen Periode (PI) der Jahre 1850 bis 1900 berechnet. Um zu untersuchen, wie stark sich die Temperatur global in den Jahren 1971 bis 2000 verändert hat, verwenden wir den HadCRUT5_ Datensatz (`Morice (2020)`_), welcher üblicherweise in GWL-Studien verwendet wird. Global ist im HadCRUT Datensatz bereits ein mittlerer Temperaturanstieg von 0,51 °K im Vergleich zum vorindustriellen Zeitraum der Jahre 1971 bis 2000 zu erkennen.

.. image:: plots/HadCRU_GWL_PI_new_version24.png

**Abbildung 3** zeigt die jährliche Anomalie der global gemittelten Temperatur im Vergleich zum vorindustriellen Zeitraum von 1850 bis 1900. Die mittlere Änderung im Referenzzeitraum von 1971 bis 2000 beträgt 0.51 K und ist eingezeichnet.

Diese Abbildung kann mit dem folgenden Notebook erstellt werden:

.. code-block:: console

   $ Notebooks/HadCru_GWL-update2024.ipynb

Es ist nicht möglich mit Hilfe der regionalen Klimasimulationen aus dem EURO-CORDEX Ensemble die Änderung zwischen dem vorindustriellen Zeitraum zu den Zeiträumen der Globalen Erwärmungsstufen zu berechnen, da das EURO-CORDEX Ensemble erst im Jahr 1971 beginnt. Als Referenzzeitraum wird daher 1971-2000 festgelegt. In diesen Untersuchungen können wir nur zeigen, wie sich das Klima während des Zeitraums einer Erwärmungstufe im Vergleich zum Referenzzeitraum verändert hat. Die Temperatur ist bereits im Referenzzeitraum angestiegen.

Ensembles für verschiedene Erwärmungsniveaus
............................................

Die Anzahl der globalen Projektionen in den Ensembles für jedes GWL variiert. Zum Beispiel erreichen die Projektionen unter Verwendung des RCP2.6 Szenarios keine globale Erwärmung von 3 °C (siehe Abbildung 4).

.. image:: plots/cmip_HadCRUt5_GWL_all_deutsch.png

**Abbildung 4** zeigt alle CMIP5 Projektionen, die im IPCC Atlas verwendet werden. Die helleren Linien repräsentieren die globalen Klimamodelle, die nicht als Antrieb in EURO-CORDEX verwendet werden, die dunkleren Linien repräsentieren die GCMs, die als Antrieb in EURO-CORDEX verwendet werden. Die als Antrieb verwendeten GCMs decken nahezu die gesamte Bandbreite der Temperaturveränderung auf globaler Ebene ab.

Diese Abbildung kann mit dem folgenden Notebook erstellt werden:

.. code-block:: console

   $ Notebooks/read_atlas_cmip5.ipynb

Die EURO-CORDEX-Projektionen werden unter Verwendung des RCP8.5 Szenarios für jedes GWL analysiert. Dadurch bleibt das Ensemble über alle GWL einigermaßen konstant. Nicht alle globalen Klimamodelle erreichen jedoch das GWL von 4 °C. Das EURO-CORDEX-Ensemble mit RCP8.5 Szenario enthält die meisten Kombinationen von globalen Klimamodellen (GCM) und regionalen Klimamodellen (RCM). Dennoch besteht eine Unsicherheit, da unterschiedliche Treibhausgasantriebe eine Wirkung haben können (`Bärring (2018)`_), insbesondere im Hinblick auf Extremereignisse. Andere Autoren empfehlen, für bestimmte Variablen alle Szenarien zu kombinieren. Weitere Informationen dazu finden sich in Querkapitel-Box 11.1 im `IPCC AR6 WG1 Chapter 11`_ .

Im folgenden werden Zeitscheiben, der globalen Erwärmsstufen der einzelen Simulationen pro RCP für das gesammte Globalmodell Ensemble des IPCC mit dem Ensemble der Globalmodelle, welche für EURO-CORDEX als Antrieb verwendet wurden, verglichen.

.. image:: plots/years_of_GWL_scenario_ensemble.png

**Abbildung 5** zeigt das zentrale Jahr der Erwärmungsstufe eines 30-Jährigen Zeitraumes für jedes Globalmodell. Es werden für jedes Szenario das Ensemble der CMIP5 Modelle (*verwendet im IPCC Atlas*) mit dem Ensemble der CMIP5 Modelle (*verwendet als Antrieb für in EURO-CORDEX*) mit einander verglichen. Die farbige Box erstreckt sich über den Bereich vom 25. bis zum 75. Perzentil, wobei der Median als schwarze Linie in der Mitte dargestellt wird. Der Median wird auch als blaue Zahl oben aufgeführt, und die schwarze Zahl unten gibt die Anzahl der Simulationen an, die das jeweilige GWL erreicht.

Diese Abbildung kann mit dem folgenden Notebook erstellt werden:

.. code-block:: console

   $ GWL_table/plot_GWL_years.ipynb

Der Vergleich der zentralen Jahre der GWL zwischen dem CMIP5-Ensemble (CMIP5) (*verwendet im IPCC Atlas*) und dem CMIP5-Ensemble (CMIP5-CORDEX) (*verwendet als Antrieb für EURO-CORDEX*) zeigt geringe Unterschiede zwischen den Szenarien für die GWL 1.5 °C und 2 °C. Für die GWL 3 °C ist der Unterschied bezüglich des Zeitraumes zwischen RCP45 und RCP85 größer als 10 Jahre. Für jedes Szenario stimmt der Median des CMIP5 Ensembles gut mit dem Median des CMIP5-CORDEX Ensembles überein. Eine Ausnahme bildet das GWL 4 °C, welches nur von einigen RCP85 Simulation erreicht wird. Hier zeigt sich ein Differenz von 8 Jahren zwischen den Medianen der beiden Ensemble.

In der Tabelle der Klimaparameter in der Broschüre *Stadtwald Karlsruhe im Klimawandel* ist der 30-Jährige Mittelwert für den Referenzzeitraum auf Grundlage von Beobachtungen (siehe vorrangehendes Kapitel) dargestellt. Der Median der Änderungen im EURO-CORDEX-Ensemble im Vergleich zum Referenzzeitraum für die verschiedenen GWL ist nur auf Grundlage des RCP85 Szenarios gezeigt, um das Ensemble über die vier GWL einigermaßen konstant zu halten.

Literatur
..........
Der beste Überblick über die unterschiedlichen Methoden zur Berechnung der globalen Erwärmungsstufen sind in `Nikulin (2018)`_ um im `IPCC`_ Atlas dargelegt. Weiterführen Information enthalten `Vautard (2014)`_ und `Kjellstroem (2017)`_.


.. _Bärring (2018): https://iopscience.iop.org/article/10.1088/1748-9326/aa9f72

.. _`Mathias Hauser`: https://github.com/mathause/cmip_warming_levels

.. _`Vautard (2014)`: https://iopscience.iop.org/article/10.1088/1748-9326/9/3/034006

.. _`Kjellstroem (2017)`: https://esd.copernicus.org/articles/9/459/2018/

.. _`Nikulin (2018)`: https://iopscience.iop.org/article/10.1088/1748-9326/aab1b1

.. _IPCC: https://github.com/IPCC-WG1/Atlas/tree/main/warming-levels

.. _HadCRUT5: https://www.metoffice.gov.uk/hadobs/hadcrut5/data/HadCRUT.5.0.2.0/download.html

.. _`IPCC Atlas`: https://github.com/IPCC-WG1/Atlas/tree/main/warming-levels

.. _`IPCC AR6 WG1 Chapter 11`: https://www.ipcc.ch/report/ar6/wg1/chapter/chapter-11/

.. _`Morice (2020)`: https://agupubs.onlinelibrary.wiley.com/doi/full/10.1029/2019JD032361

.. _`Unterschied`: https://github.com/IPCC-WG1/Atlas/blob/main/warming-levels/CMIP5_WarmingLevels_spread_RCP85.pdf
