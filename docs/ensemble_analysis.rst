Berechnung der Signifikanz und Robustheit
-----------------------------------------

Ein Ensemble von Klimasimulationen wird verwendet, um die Unsicherheit in den Modellprojektionen zu berücksichtigen und die Robustheit der Ergebnisse zu erhöhen. 

Klimamodelle sind vereinfachte Darstellungen des realen Klimasystems und beruhen auf verschiedenen Annahmen und Parametern. Durch die Verwendung eines Ensembles können verschiedene Modelle mit unterschiedlichen Parametern berücksichtigt werden, um die Bandbreite der möglichen Ergebnisse zu erfassen und die Unsicherheit zu reduzieren.

Die statistische Signifikanz der Klimaänderung wird für jede einzelne Klimasimulation berechnet.  Dies geschieht mit einem statistischen Testverfahren, das bewertet, ob eine gegebene Veränderung so stark ist, dass sie die zufälligen (natürlichen) Schwankungen übersteigt. Eine Klimaänderung wird hier als signifikant definiert, wenn sie gemäß eines sogenannten Mann-Whitney-U-Tests mit einer Wahrscheinlichkeit von unter 5% mit zufälligen Schwankungen erklärbar ist.

Experteneinschätzung
....................

Die Ergebnisse des ausgewählten Modellensembles sind mit Signifikanz und Robustheit versehen. Die berechnung wurde unter Verwendung von xclim_ durchgeführt.

**Robuste-Zunahme**: Mindestens 2/3 der Simulationen zeigen eine Zunahme und mindestens 50% der Simulationen sogar eine significante Zunahme.

**Robuste-Abnahme**:  Mindestens 2/3 der Simulationen zeigen eine Abnahme und mindestens 50% der Simulationen sogar eine signifikante Abnahme.

**Tendenz zur Zunahme:** Mindestens 2/3 der Simulationen zeigen eine Zunahme, aber weniger als 50% der Simulationen eine signifikante Zunahme.

**Tendenz zur Abnahme:** Mindestens 2/3 der Simulationen zeigen eine Abnahme, aber weniger als 50% der Simulationen eine signifikante Abnahme.

**Unklar:** Keine 2/3-Mehrheit bezüglich der Richtung der Änderungen, aber mindestens 50% der Simulationen zeigen signifikante Änderungen.

**Keine Änderungen:** Keine 2/3-Mehrheit bezüglich der Richtung der Änderungen; weniger als 50% der Simulationen zeigen signifikante Änderungen


.. _xclim: https://github.com/Ouranosinc/xclim
