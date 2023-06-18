---
share: true
---

## Was Ist Git?

Git ist ein Versionskontrollsystem, das entwickelt wurde, um die Verwaltung von Änderungen in Softwareprojekten zu erleichtern. Es ermöglicht Entwicklern, ihre Arbeit zu verfolgen, Änderungen zu verwalten und effektiv mit anderen zusammenzuarbeiten.

### ELI5

Stell dir vor, du malst ein Bild auf einem Blatt Papier. Aber du möchtest nicht nur das fertige Bild behalten, sondern auch den gesamten Entstehungsprozess aufzeichnen, um später Änderungen vornehmen oder auf ältere Versionen zurückgreifen zu können. Hier kommt Git ins Spiel.

Git ist wie ein magisches Tagebuch für deine Arbeit an einem Projekt. Jedes Mal, wenn du Änderungen an deinem Projekt vornimmst, schreibst du sie in das Tagebuch auf. Git speichert jede Version deiner Dateien und speichert alle Änderungen, die du machst.

Mit Git kannst du verschiedene Versionen deiner Dateien erstellen, so ähnlich wie wenn du ein Bild in verschiedenen Schritten malst. Du kannst den Fortschritt sehen und zu jedem beliebigen Zeitpunkt zu einer früheren Version zurückkehren.

Git hilft auch beim Zusammenarbeiten mit anderen. Stell dir vor, du möchtest mit einem Freund zusammen an demselben Bild arbeiten. Git erlaubt euch beiden, an euren eigenen Kopien des Projekts zu arbeiten und die Änderungen später zu kombinieren. Es sorgt dafür, dass ihr nicht versehentlich eure Arbeit überschreibt.

Git ist wie ein Zauberbuch, das deine Arbeit speichert, Veränderungen verfolgt und es dir ermöglicht, alle früheren Versionen deiner Dateien zu behalten. Es ist ein leistungsstarkes Werkzeug für Entwickler und Künstler, um ihre Arbeit zu organisieren und effektiv zusammenzuarbeiten.

## Versionierung

Versionierung bezieht sich auf die Verwaltung und Nachverfolgung von Änderungen an Dateien oder Code. Mit Git kannst du den Verlauf deiner Änderungen speichern und auf frühere Versionen zurückgreifen, falls etwas schief geht oder du zu einer früheren Version zurückkehren möchtest.

## Branches

Branches sind separate Linien der Entwicklung in einem Git-Repository. Sie erlauben es Entwicklern, unabhängig voneinander an unterschiedlichen Funktionen oder Aufgaben zu arbeiten. Jeder Branch hat eine eigene Kopie des Codes, auf der Änderungen gemacht werden können, ohne die Hauptentwicklungslinie zu beeinflussen.

### Beispiel

![Example](https://ardalis.com/img/image-git-graph.png)

## Merge

Merge ist der Prozess, bei dem Änderungen aus einem Branch in einen anderen Branch oder in den Hauptentwicklungszweig (oft als "master" oder "main" bezeichnet) überführt werden. Es kombiniert die Änderungen und integriert sie nahtlos, so dass der Code auf dem aktuellen Stand ist.

## Fetch

Fetch all bezieht sich auf den Vorgang, bei dem alle Änderungen und Updates aus einem entfernten Git-Repository abgerufen werden. Das umfasst sowohl neue Branches als auch Änderungen an vorhandenen Branches.

## Rebase

Rebase ist ein Git-Befehl, der es ermöglicht, die Änderungen in einem Branch auf den neuesten Stand zu bringen, indem sie auf die neueste Version des Hauptentwicklungszweigs angewendet werden. Dadurch entsteht ein linearerer Verlauf der Änderungen im Code.

## Repository

Ein Repository ist ein Speicherort, in dem Git den Code und die Dateien eines Projekts speichert. Es enthält den gesamten Verlauf der Änderungen, die verschiedenen Branches und alle Informationen, die zum Verwalten des Codes benötigt werden.

## GitHub

GitHub ist eine webbasierte Plattform, die auf Git basiert und es Entwicklern ermöglicht, ihre Git-Repositories online zu hosten und mit anderen zusammenzuarbeiten. Es bietet Funktionen wie Pull Requests, um Änderungen zu überprüfen und zu integrieren, Issue Tracking für das Verfolgen von Aufgaben und Fehlermeldungen, sowie Tools für die Zusammenarbeit in Teams. Es ist eine beliebte Plattform für die gemeinsame Entwicklung von Open-Source-Projekten und für die Zusammenarbeit in Softwareentwicklungsteams.

## Pull Request

Ein Pull Request ist ein Beitrag, den ein Entwickler zu einem Softwareprojekt leistet. Der Entwickler ändert den Code auf seinem eigenen Fork oder einer Kopie des Projekts und stellt dann eine Anfrage, um diese Änderungen in das Hauptprojekt einzufügen. Andere Mitglieder des Teams können die Änderungen prüfen, kommentieren und Vorschläge zur Verbesserung machen, bevor sie in das Hauptprojekt eingefügt werden.

## Codeowners

Die CODEOWNERS Datei in einem GitHub-Projekt wird genutzt, um bestimmte Personen oder Teams automatisch als Reviewer für Pull Requests einzusetzen, die bestimmte Dateien oder Verzeichnisse betreffen.

## Review-Prozess

Der Review-Prozess in Softwareentwicklung bezieht sich auf den Prozess, in dem andere Entwickler den Code prüfen, der in einem Pull Request vorgeschlagen wurde. Sie überprüfen die Qualität des Codes, ob er die Problemstellung korrekt löst, ob er keine neuen Fehler oder Sicherheitsprobleme einführt, usw. Dieser Prozess ist eine wichtige Methode, um Codequalität und Konsistenz in einem Softwareprojekt zu gewährleisten.

## Master/Main

In Git, einer weit verbreiteten Versionskontrollsoftware, waren "master" der Standardname für den Hauptzweig, in den alle Features und Änderungen letztendlich eingefügt werden. Allerdings hat sich die Community dahingehend bewegt, "main" anstelle von "master" zu verwenden, um problematische Konnotationen des Begriffs "master" zu vermeiden. Beide Begriffe beziehen sich also auf den Hauptzweig eines Git-Projekts, aber "main" ist der aktuell bevorzugte Begriff.

## Geschützte Branches (Protected Branches)

In Git können bestimmte Branches als "geschützt" gekennzeichnet werden. Dies bedeutet, dass für diese Branches besondere Regeln gelten, um zu verhindern, dass sie versehentlich oder schädlich verändert werden. Zum Beispiel könnte ein geschützter Branch das Löschen oder das direkte Pushen ohne Pull Request verhindern. Insbesondere der Hauptzweig eines Projekts (master/main) ist oft ein geschützter Branch.
