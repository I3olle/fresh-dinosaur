---
share: true
---

## Stages

Im Kontext der Softwareentwicklung bezeichnet "Stages" oder "Phasen" die unterschiedlichen Schritte im Entwicklungsprozess eines Softwareprodukts. Häufig genutzte Phasen sind beispielsweise Planung, Design, Implementierung, Testen, Deployment und Wartung. Jede Phase hat einen spezifischen Fokus und Zweck innerhalb des gesamten Lebenszyklus der Softwareentwicklung. Manchmal können diese Phasen linear ablaufen (wie im Wasserfallmodell), aber in agilen oder iterativen Entwicklungsansätzen können sie sich auch überlappen oder wiederholen.

## SDLC

SDLC steht für "Software Development Life Cycle" und bezeichnet den Prozess, den ein Softwareprodukt von der ursprünglichen Konzeption bis zur endgültigen Auslieferung und Wartung durchläuft. Es gibt verschiedene Modelle für den SDLC, darunter das Wasserfallmodell, das Spiralmodell und agile Modelle. Jedes Modell hat verschiedene Phasen oder "Stages", die in unterschiedlicher Reihenfolge und auf unterschiedliche Weise durchlaufen werden. Im Allgemeinen umfasst der SDLC Phasen wie Anforderungsanalyse, Design, Implementierung, Testen, Deployment und Wartung.


Siehe [Git](./Git.md#)
![Git > Review-Prozess](./Git.md#review-prozess)

## Semantic Versioning

Semantic Versioning, oft auch als SemVer bezeichnet, ist ein Versionierungsschema, das versucht, Bedeutung zu den Versionen von Software zu bringen. Es hilft dabei, Veränderungen an der Software klar zu kommunizieren und den Erwartungen der Nutzer gerecht zu werden.

Ein typisches SemVer-Format besteht aus drei Zahlen, die durch Punkte getrennt sind. Diese drei Zahlen repräsentieren die Hauptversion (major), Nebenversion (minor) und den Patchstand (patch). Das Format sieht also wie folgt aus:

```
MAJOR.MINOR.PATCH
```

Hier ist, was jede dieser Komponenten bedeutet:

- **MAJOR**: Diese Zahl erhöht sich, wenn es inkompatible Änderungen in der API gibt, die dazu führen, dass Nutzer ihre Art der Nutzung der Software ändern müssen, um mit dieser neuen Version zu arbeiten.

- **MINOR**: Diese Zahl erhöht sich, wenn es neue Funktionen gibt, die abwärtskompatibel sind. Das bedeutet, dass Nutzer neue Funktionen nutzen können, ohne dass sie ihre Art der Nutzung der Software ändern müssen.

- **PATCH**: Diese Zahl erhöht sich, wenn abwärtskompatible Bugfixes durchgeführt wurden. Das sind in der Regel kleinere Änderungen, die vorhandene Probleme beheben, ohne die Art und Weise, wie die Software genutzt wird, zu ändern.

Darüber hinaus können Prerelease- und Build-Metadaten durch einen Bindestrich bzw. Pluszeichen an das Ende des Formats angehängt werden. Sie sind optional und bieten weitere Details über die Version.

Ein Beispiel für ein vollständiges SemVer-Format könnte 2.5.0-alpha+001 sein. Hierbei handelt es sich um die Hauptversion 2, Nebenversion 5, Patch 0, eine Alpha-Vorabversion und Build 001.
