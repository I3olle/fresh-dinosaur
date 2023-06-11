---
share: true
---

# Konzepte

## Serverless

Serverless ist ein Konzept in der Cloud-Computing-Architektur, bei dem der Entwickler nicht die physischen Server verwalten muss, sondern sich auf die Ausführung des Codes konzentrieren kann. Obwohl der Name "serverless" (serverfrei) impliziert, dass keine Server involviert sind, gibt es tatsächlich immer noch Server, die den Code ausführen. Der Unterschied besteht jedoch darin, dass das Management der Server von den Cloud-Anbietern und nicht von den Entwicklern oder ihren Organisationen durchgeführt wird. AWS Lambda ist ein Beispiel für eine serverless Plattform.

Die Idee hinter der serverless Architektur besteht darin, Entwickler von der Notwendigkeit zu befreien, sich um das Hosting und die Skalierung ihrer Anwendungen kümmern zu müssen. Stattdessen können sie sich auf das Schreiben des Codes konzentrieren, während der Cloud-Anbieter (wie AWS, Google Cloud oder Azure) sich um das Hosting und die Skalierung kümmert. Das bedeutet auch, dass die Kosten im Allgemeinen variabel sind und auf dem tatsächlichen Verbrauch basieren, anstatt dass feste Kosten für die Serverkapazität anfallen.

### ELI5

Okay, lass uns versuchen, Serverless so einfach wie möglich zu erklären.

Stell dir vor, du möchtest eine Geburtstagsparty veranstalten, aber du hast keine Lust, alles selbst zu organisieren - du willst nicht den Raum mieten, die Dekorationen aufhängen, das Essen zubereiten, und so weiter. Stattdessen gehst du zu einem Veranstaltungsort, der alles für dich erledigt. Sie haben den Raum, sie bereiten das Essen zu, sie kümmern sich um die Dekoration - alles, was du tun musst, ist aufzutauchen und die Party zu genießen. Und das Beste daran? Du bezahlst nur für das, was du tatsächlich nutzt.

Serverless ist ähnlich, aber für Computerprogramme. Statt einen eigenen Computer (Server) zu haben, der immer bereit ist und läuft, um dein Programm auszuführen, lädst du einfach dein Programm in die "Cloud" hoch (das ist ein anderer Name für Computer, die von großen Unternehmen wie Amazon, Google oder Microsoft betrieben werden). Diese Unternehmen kümmern sich um alles - sie sorgen dafür, dass dein Programm immer dann läuft, wenn es benötigt wird, sie sorgen dafür, dass es mehr Ressourcen hat, wenn es sehr beschäftigt ist, und sie sorgen dafür, dass es sicher ist. Und genau wie bei der Geburtstagsparty bezahlst du nur für das, was du tatsächlich nutzt.

Das ist der Grundgedanke hinter Serverless - es ermöglicht Entwicklern, sich auf ihr Programm zu konzentrieren, ohne sich um all die Details kümmern zu müssen, die mit dem Betrieb eines Servers verbunden sind.

## Microservices

Microservices, auch bekannt als Mikroservice-Architektur, sind ein architektonischer Ansatz für die Softwareentwicklung, bei dem eine Anwendung aus kleinen, unabhängigen Services besteht, die jeweils einen spezifischen Geschäftsprozess oder eine Geschäftsfunktion ausführen.

Jeder Microservice in einer Anwendung ist ein eigenständiger Prozess, der eine spezifische Geschäftsfunktion erfüllt und über eine gut definierte API kommuniziert. Microservices können unabhängig voneinander entwickelt, bereitgestellt und skaliert werden, und sie können in unterschiedlichen Programmiersprachen geschrieben und auf unterschiedlichen Plattformen ausgeführt werden.

Hier sind einige Vorteile der Verwendung von Microservices:

- **Entkopplung**:
	- Da jeder Microservice für eine bestimmte Funktion zuständig ist, können Änderungen an einem Service vorgenommen werden, ohne andere Services zu beeinflussen. Dies kann die Entwicklungsgeschwindigkeit und -flexibilität erhöhen.
- **Skalierbarkeit**:
	- Microservices können unabhängig voneinander skaliert werden, je nachdem, welcher Service gerade die höchste Last hat. Dies kann dazu beitragen, Ressourcen effizienter zu nutzen und die Leistung der Anwendung zu verbessern.
- **Fehlertoleranz**:
	- Wenn ein Microservice ausfällt, beeinträchtigt das normalerweise nicht den Rest der Anwendung. Dies kann dazu beitragen, die Gesamtverfügbarkeit und Zuverlässigkeit der Anwendung zu verbessern.
- **Technologische Vielfalt**:
	- Da Microservices unabhängig voneinander entwickelt werden können, haben Teams die Freiheit, die Technologien zu wählen, die am besten zu den Anforderungen jedes einzelnen Services passen.

Trotz dieser Vorteile bringt die Microservice-Architektur auch Herausforderungen mit sich, insbesondere in Bezug auf die Verwaltung und Orchestrierung einer größeren Anzahl von Services, das Monitoring und Debugging von Problemen in einem verteilten System, und die Aufrechterhaltung der Datenintegrität über mehrere Datenbanken hinweg. Es ist wichtig, diese Herausforderungen zu berücksichtigen und geeignete Tools und Praktiken einzusetzen, wenn man sich für eine Microservice-Architektur entscheidet.

### ELI5

Stell dir vor, du hast einen riesigen Lego-Bausatz. Du könntest alle Teile in einen großen Haufen werfen und versuchen, das Modell so zu bauen. Aber es wäre viel einfacher, wenn du die Teile in kleine Haufen aufteilst, die jeweils zu einem bestimmten Abschnitt des Modells gehören. So könntest du jeden Abschnitt einzeln bauen, und wenn du einen Fehler machst oder etwas ändern möchtest, musst du nur den betreffenden Abschnitt ändern und nicht das gesamte Modell.

Microservices in der Softwareentwicklung funktionieren ähnlich. Anstatt eine große, komplexe Anwendung zu haben, teilen wir sie auf in viele kleinere Dienste (ähnlich wie die kleinen Haufen von Lego-Teilen), wobei jeder Dienst für eine bestimmte Aufgabe zuständig ist. Diese Dienste arbeiten zusammen, um die gesamte Anwendung zu bilden, aber weil sie unabhängig voneinander sind, können wir sie einzeln ändern oder verbessern, ohne die gesamte Anwendung beeinflussen zu müssen.

Diese Art der Organisation macht es einfacher, große und komplexe Anwendungen zu erstellen und zu verwalten, da wir uns auf einzelne Teile konzentrieren können, statt immer die gesamte Anwendung im Blick haben zu müssen. Es ist auch einfacher, Probleme zu beheben, da wir uns auf den spezifischen Dienst konzentrieren können, der das Problem verursacht, anstatt durch den gesamten Code der Anwendung suchen zu müssen.

# Tools

## Lambda

AWS Lambda ist ein Dienst von Amazon Web Services (AWS), der es Ihnen ermöglicht, Code auszuführen, ohne dass Sie Server bereitstellen oder verwalten müssen. Mit AWS Lambda laden Sie einfach Ihren Code hoch (der eine Funktion oder "Lambda-Funktion" genannt wird), und der Dienst führt ihn aus, wann immer der definierte Trigger (wie eine Änderung in einer Datenbank, eine Anfrage an eine API oder ein bestimmtes Ereignis) aktiviert wird. Sie zahlen nur für die Rechenzeit, die Sie tatsächlich verbrauchen, was Lambda und ähnliche Dienste zu einer kosteneffizienten Wahl für viele Anwendungen macht.
