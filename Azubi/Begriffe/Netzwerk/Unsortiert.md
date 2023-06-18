---
share: true
---


Beschtes Video von "Die Sendung mit der Maus"
<https://youtu.be/fpqhjEtznVk?t=76>


Man kann die einzelnen Begriffe definitiv besser strukturieren. Vorerst werden hier die jeweiligen Begriffe gesammelt die noch nicht zu einer eigenen Unterkategorie gehören.

## Ports

Ports sind nummerierte Kanäle auf einem Gerät, die bestimmten Anwendungen oder Diensten zugeordnet werden. Ports ermöglichen die gleichzeitige Kommunikation mehrerer Anwendungen über das Netzwerk. Sie werden oft mit der IP-Adresse kombiniert, um eine bestimmte Anwendung auf einem bestimmten Gerät zu identifizieren. Ein Port wird durch eine 16-Bit-Zahl dargestellt und kann Werte von 0 bis 65535 haben. Es gibt bestimmte Standardports, die für bestimmte Dienste reserviert sind, wie z. B. Port 80 für HTTP (Hypertext Transfer Protocol) oder Port 443 für HTTPS (Hypertext Transfer Protocol Secure).

### ELI5

Stell dir vor, du möchtest eine wichtige Nachricht an einen Freund schicken. Du weißt, dass dein Freund in einem großen Gebäude wohnt, das viele verschiedene Räume hat. Aber wie findest du heraus, in welchem Raum sich dein Freund befindet?

Hier kommen Ports ins Spiel. Stell dir vor, das Gebäude hat viele Türen, und jede Tür hat eine Nummer. Jeder Raum in dem Gebäude hat eine bestimmte Funktion oder Aufgabe. Ein Port ist wie eine Tür mit einer Nummer, die zu einem bestimmten Raum führt.

Wenn du eine Nachricht an deinen Freund senden möchtest, musst du wissen, welchen Raum er sich gerade aufhält. Indem du die richtige Tür mit der passenden Nummer benutzt, kannst du sicherstellen, dass deine Nachricht den richtigen Raum erreicht.

Im Computerbereich funktioniert es ähnlich. Ein Port ist eine Nummer, die einem bestimmten Dienst oder einer bestimmten Anwendung auf einem Computer zugeordnet ist. Wenn Daten von einem Gerät zu einem anderen über das Netzwerk gesendet werden, müssen sie wissen, welchen Port sie erreichen müssen, um zur richtigen Anwendung oder zum richtigen Dienst zu gelangen.

Es gibt Tausende von Ports, die für verschiedene Zwecke reserviert sind. Einige Ports sind Standardports, die für bestimmte Dienste reserviert sind. Zum Beispiel ist Port 80 der Standardport für unverschlüsselte Webseiten (HTTP), während Port 443 für verschlüsselte Webseiten (HTTPS) verwendet wird. Port 22 wird oft für sichere Fernzugriffsverbindungen (SSH) verwendet.

Ports sind also wie die Nummern an den Türen in einem großen Gebäude. Sie helfen dabei, Datenpakete an die richtigen Anwendungen oder Dienste auf Computern zu senden, wenn sie über das Netzwerk kommunizieren.

## DNS

DNS steht für Domain Name System. Es ist wie ein Telefonbuch des Internets, das hilft, die Namen von Websites in die zugehörigen IP-Adressen zu übersetzen.

Stell dir vor, du möchtest eine Website wie "[www.beispiel.com](http://www.beispiel.com/)" besuchen. Aber Computer kommunizieren über IP-Adressen, wie z. B. 192.168.0.1. Hier kommt DNS ins Spiel.

Das DNS-System besteht aus Servern und Protokollen, die die Namensauflösung ermöglichen. Wenn du den Namen einer Website eingibst, sendet dein Computer eine Anfrage an den DNS-Server. Der DNS-Server übersetzt dann den Namen in die entsprechende IP-Adresse und gibt sie an deinen Computer zurück.

DNS ist wichtig, weil es den Menschen ermöglicht, sich leicht an Namen wie "beispiel.com" zu erinnern, anstatt sich IP-Adressen merken zu müssen. Es vereinfacht die Kommunikation im Internet und ermöglicht es uns, Websites über ihre Namen zu erreichen.

Zusammenfassend gesagt ist DNS ein System, das die Namen von Websites in die zugehörigen IP-Adressen übersetzt. Es macht es einfacher, Websites über Namen statt über IP-Adressen zu erreichen und spielt eine wichtige Rolle bei der Kommunikation im Internet.

## API

API steht für "Application Programming Interface". Es handelt sich dabei um eine Sammlung von Regeln und Protokollen, die festlegen, wie verschiedene Softwareanwendungen oder -komponenten miteinander interagieren und kommunizieren sollen. Sie können sich eine API als eine Art Speisekarte in einem Restaurant vorstellen. Die Speisekarte bietet eine Liste von Gerichten, die Sie bestellen können, zusammen mit einer Beschreibung dessen, was jedes Gericht beinhaltet. In ähnlicher Weise definiert eine API eine Liste von Funktionen oder Diensten, die von einer Softwareanwendung bereitgestellt werden, zusammen mit Anweisungen darüber, wie diese Funktionen oder Dienste verwendet werden können.

Es gibt verschiedene Arten von APIs, aber hier sind ein paar Beispiele, um Ihnen eine Vorstellung zu geben:

- **Web-APIs**
	- oft auch als HTTP-APIs oder REST-APIs bezeichnet, ermöglichen die Kommunikation zwischen verschiedenen Softwareanwendungen über das Internet. Zum Beispiel könnte eine Wetter-App eine Web-API verwenden, um Wetterdaten von einem Server abzurufen.
- **Betriebssystem-APIs**
	- definieren, wie Anwendungen mit einem Betriebssystem interagieren können. Zum Beispiel könnte eine Anwendung eine Betriebssystem-API verwenden, um ein Fenster auf dem Bildschirm zu öffnen oder um Zugriff auf Dateien auf der Festplatte zu erhalten.
- **Bibliothekoder Framework-APIs**
	- definieren, wie Anwendungen mit einer bestimmten Softwarebibliothek oder einem Framework interagieren können. Zum Beispiel könnte eine Anwendung eine Bibliotheks-API verwenden, um komplexe mathematische Berechnungen durchzuführen oder um eine Datenbank abzufragen.

APIs sind ein grundlegender Baustein der modernen Softwareentwicklung und ermöglichen es Entwicklern, komplexe Anwendungen zu erstellen, die auf den Funktionen und Diensten aufbauen, die von anderen zur Verfügung gestellt werden.

### API Call

Ein API-Call ist eine Anfrage, die an eine API (Application Programming Interface) gesendet wird, um eine bestimmte Funktion auszuführen. APIs sind im Grunde genommen eine Art von Vertrag zwischen verschiedenen Softwareanwendungen, die festlegt, wie sie miteinander kommunizieren und Daten austauschen können.

Ein API-Call besteht normalerweise aus mehreren Teilen:

- **Die Basis-URL**:
	- Dies ist die grundlegende Webadresse, an die der Call gesendet wird.
- **Der Endpunkt**:
	- Dies ist der spezifische Pfad an der Basis-URL, der auf eine bestimmte Ressource oder eine Sammlung von Ressourcen verweist.
- **Die Methode**:
	- Dies gibt an, welche Art von Aktion ausgeführt werden soll. In einer RESTful API, einer der gebräuchlichsten Arten von APIs, gibt es meist vier Methoden: GET (Daten abrufen), POST (neue Daten erstellen), PUT oder PATCH (bestehende Daten aktualisieren) und DELETE (Daten löschen).
- **Die Parameter oder der Body**:
	- Dies sind zusätzliche Informationen, die mit dem API-Call gesendet werden können. Bei einem GET-Request könnten dies zum Beispiel Suchparameter sein, die angeben, welche Daten genau abgerufen werden sollen. Bei einem POST-, PUToder PATCH-Request könnte es sich um die tatsächlichen Daten handeln, die erstellt oder aktualisiert werden sollen.

So könnte beispielsweise ein API-Call an eine Wetter-API aussehen: `GET https://api.weather.com/v3/wx/forecast/daily/5day?apiKey=YOUR_API_KEY&geocode=37.7,-122.4`. Dieser Call verwendet die GET-Methode, um die 5-Tage-Wettervorhersage für die geographischen Koordinaten 37.7,-122.4 (San Francisco) von der `api.weather.com` API abzurufen.

## Cloudfront

Amazon CloudFront ist ein Content-Delivery-Network (CDN) Service, der von Amazon Web Services (AWS) angeboten wird. Ein CDN ist ein Netzwerk verteilter Server, die Inhalte zu Nutzern basierend auf deren geografischer Lage ausliefern.

Die Hauptfunktion von CloudFront ist es, Daten, Videos, Anwendungen und APIs sicher und mit hoher Geschwindigkeit und geringer Latenz an Nutzer weltweit zu liefern. CloudFront ist tief in das AWS-Netzwerk integriert, was es zu einem geeigneten CDN für die Lieferung von Inhalten macht, die in anderen AWS-Diensten gehostet werden, wie z.B. in Amazon S3 (Simple Storage Service), Amazon EC2 (Elastic Compute Cloud) oder AWS Elastic Load Balancing.

Einige der Hauptfunktionen von CloudFront umfassen:

- **Edge Locations**: CloudFront verwendet ein Netzwerk von "Edge Locations" auf der ganzen Welt, um Inhalte näher an die Nutzer zu bringen, was die Latenz reduziert. Wenn ein Nutzer eine Anfrage an einen Inhalt stellt, wird die Anfrage an die nächstgelegene Edge Location weitergeleitet, um eine schnelle Lieferung zu gewährleisten.

- **Caching**: CloudFront speichert Kopien von Inhalten (d.h. es erstellt ein Cache) an diesen Edge Locations, so dass wiederholte Anfragen nach dem gleichen Inhalt schneller bedient werden können, ohne dass die Anfrage jedes Mal bis zum Ursprungsserver zurückgehen muss.

- **Sicherheit**: CloudFront bietet Sicherheitsfunktionen wie SSL/TLS für sichere Netzwerkverbindungen, AWS Shield für DDoS-Schutz und AWS WAF (Web Application Firewall) für den Schutz vor webbasierten Bedrohungen. Darüber hinaus unterstützt es auch die Anforderungen des Identity and Access Management (IAM) von AWS.

- **Integration**: Wie bereits erwähnt, ist CloudFront tief in das AWS-Ökosystem integriert, was bedeutet, dass es einfach ist, es mit anderen AWS-Diensten zu verwenden, und es ist auch einfach, mit CloudFront über die AWS-Managementkonsole, CLI (Command Line Interface) und SDKs (Software Development Kits) zu interagieren.

Das sind nur einige der Funktionen von Amazon CloudFront. Es bietet auch Unterstützung für benutzerdefinierte SSL-Zertifikate, das Streaming von Live- und On-Demand-Videos, und es ist kompatibel mit mehreren Protokollen, einschließlich HTTP, HTTPS, RTMP und mehr.