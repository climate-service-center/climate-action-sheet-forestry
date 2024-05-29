Berechnung von Signifikanz und Robustheit der Klimaänderung
-----------------------------------------------------------

Ein Ensemble von Klimasimulationen wird verwendet, um die Unsicherheit in den Modellprojektionen zu berücksichtigen und die Robustheit der Ergebnisse zu erhöhen.

Die Unsicherheiten_ in der Klimamodellierung resultieren aus der Komplexität des Klimasystems mit seinen Wechselwirkungen, den erforderlichen Vereinfachungen der Klimaprozesse in den Modellen (computerbedingte numerische Parametrisierung), der natürlichen Klimavariabilität und den Annahmen über die zukünftigen Entwicklungen der Treibhausgaskonzentrationen, der Aerosole und der Landnutzung.

Die statistische Signifikanz der Klimaänderung wird für jede einzelne Klimasimulation berechnet.  Dies geschieht mit einem statistischen Testverfahren, das bewertet, ob eine gegebene Veränderung so stark ist, dass sie die zufälligen (natürlichen) Schwankungen übersteigt. Eine Klimaänderung wird hier als signifikant definiert, wenn sie gemäß eines sogenannten `Mann-Whitney-U-Tests`_ mit einer Wahrscheinlichkeit von unter 5% mit zufälligen Schwankungen erklärbar ist.

Experteneinschätzung
....................

Die Ergebnisse des ausgewählten Modellensembles sind mit Informationen zu Signifikanz und Robustheit versehen. Die Berechnung wurde unter Verwendung von xclim_ durchgeführt.

**Robuste-Zunahme**: Mindestens 2/3 der Simulationen zeigen eine Zunahme und mindestens 50% der Simulationen sogar eine signifikante Zunahme.

**Robuste-Abnahme**:  Mindestens 2/3 der Simulationen zeigen eine Abnahme und mindestens 50% der Simulationen sogar eine signifikante Abnahme.

**Tendenz zur Zunahme:** Mindestens 2/3 der Simulationen zeigen eine Zunahme, aber weniger als 50% der Simulationen eine signifikante Zunahme.

**Tendenz zur Abnahme:** Mindestens 2/3 der Simulationen zeigen eine Abnahme, aber weniger als 50% der Simulationen eine signifikante Abnahme.

**Unklar:** Keine 2/3-Mehrheit bezüglich der Richtung der Änderungen, aber mindestens 50% der Simulationen zeigen signifikante Änderungen.

**Keine Änderungen:** Keine 2/3-Mehrheit bezüglich der Richtung der Änderungen; weniger als 50% der Simulationen zeigen signifikante Änderungen


.. _xclim: https://github.com/Ouranosinc/xclim

.. _`Mann-Whitney-U-Tests`: https://de.wikipedia.org/wiki/Wilcoxon-Mann-Whitney-Test

.. _`Unsicherheiten`: https://link.springer.com/chapter/10.1007/978-3-662-66696-8_5#Sec3
