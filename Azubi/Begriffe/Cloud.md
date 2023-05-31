---
share: true  
--- 
# Cloud
Die Cloud ist ein Begriff, der sich auf eine virtuelle Umgebung bezieht, in der Ressourcen und Dienste über das Internet bereitgestellt werden. Statt lokale Server und Infrastruktur zu verwenden, können Unternehmen und Benutzer die Cloud nutzen, um auf leistungsstarke Rechenkapazitäten, Speicherplatz, Datenbanken, Netzwerke und viele andere Dienste zuzugreifen. Die Cloud bietet Skalierbarkeit, Flexibilität und die Möglichkeit, Ressourcen nach Bedarf zu nutzen, ohne in teure Hardware investieren zu müssen.


> [!NOTE] Info
> Da ich fast ausschließlich mit der AWS Cloud arbeite, werden sich auch die meisten Cloud Themen auf die AWS Cloud beziehen



## AWS Accounts
AWS Accounts sind Konten, die von Amazon Web Services (AWS) bereitgestellt werden. Mit einem AWS Account können Benutzer auf die verschiedenen Dienste und Ressourcen von AWS zugreifen. Jeder AWS Account hat eine eindeutige Kennung und kann verwendet werden, um Ressourcen in der AWS-Cloud zu erstellen, zu verwalten und darauf zuzugreifen.


## VPC
VPC steht für Virtual Private Cloud und ist ein Dienst von AWS, der es Benutzern ermöglicht, eine isolierte, virtuelle Netzwerkumgebung in der AWS-Cloud zu erstellen. Eine VPC fungiert als abgeschottetes Netzwerk, in dem Benutzer ihre Ressourcen betreiben können. Es erlaubt die Kontrolle über das Netzwerkdesign, die IP-Adressierung, die Subnetze und die Netzwerksicherheit. Mit einer VPC können Benutzer ihre Infrastruktur in der Cloud maßgeschneidert konfigurieren und verwalten, während sie gleichzeitig eine isolierte Umgebung erhalten, um ihre Anwendungen und Daten zu schützen.


## Security Groups
Security Groups sind ein Sicherheitsmechanismus in der AWS-Cloud, der den Zugriff auf Ressourcen innerhalb einer Virtual Private Cloud (VPC) kontrolliert. Sie fungieren als virtuelle Firewalls und ermöglichen es Benutzern, den eingehenden und ausgehenden Netzwerkverkehr für ihre Ressourcen zu steuern.

Eine Security Group ist mit einer oder mehreren Instanzen (z. B. EC2-Instanzen) oder anderen AWS-Ressourcen verknüpft. Sie besteht aus Regeln, die den Netzwerkverkehr basierend auf Quell- und Ziel-IP-Adressen, Ports und Protokollen steuern. Diese Regeln definieren, welche Arten von Verbindungen erlaubt oder blockiert werden.

Security Groups arbeiten auf dem Prinzip der "Deny-by-default"-Regel, was bedeutet, dass der gesamte eingehende Verkehr standardmäßig blockiert wird, es sei denn, es wurden explizite Regeln definiert, die den Verkehr zulassen. Dadurch wird ein höheres Maß an Sicherheit gewährleistet, da nur der spezifizierte erlaubte Verkehr zugelassen wird.

Benutzer können die Regeln einer Security Group flexibel konfigurieren und anpassen, um den spezifischen Sicherheitsanforderungen ihrer Anwendungen gerecht zu werden. Zum Beispiel können sie festlegen, dass nur bestimmte IP-Adressen oder IP-Bereiche auf bestimmte Ports zugreifen dürfen.

Security Groups sind ein wesentlicher Bestandteil der Sicherheitsarchitektur in der AWS-Cloud. Sie helfen dabei, den Zugriff auf Ressourcen zu kontrollieren, potenzielle Angriffe abzuwehren und die Integrität und Vertraulichkeit von Daten in der Cloud zu gewährleisten. Durch die korrekte Konfiguration und Verwaltung von Security Groups können Benutzer ihre Ressourcen effektiv vor unberechtigtem Zugriff schützen.

### ELI5
Stell dir vor, du möchtest eine Party in deinem Haus feiern. Damit die Party sicher und geschützt ist, möchtest du kontrollieren, wer in dein Haus darf und wer nicht. Hier kommen Security Groups ins Spiel.

Eine Security Group ist wie ein Sicherheitsdienst für dein Haus. Sie hilft dir dabei, den Zugriff auf deine Ressourcen in der AWS-Cloud zu kontrollieren. Du kannst festlegen, wer von außen auf deine Ressourcen zugreifen darf und wer nicht.

Ähnlich wie bei einer Gästeliste kannst du mit einer Security Group bestimmte Regeln festlegen. Zum Beispiel kannst du sagen: "Nur meine Freunde dürfen zur Party kommen" oder "Niemand darf nach 22 Uhr in mein Haus".

In der AWS-Cloud funktioniert es ähnlich. Du kannst eine Security Group erstellen und Regeln definieren, wer auf deine Ressourcen zugreifen darf und wer nicht. Du kannst den Zugriff auf bestimmte IP-Adressen oder IP-Bereiche, bestimmte Ports oder bestimmte Protokolle beschränken.

Wenn jemand versucht, auf deine Ressourcen zuzugreifen, überprüft die Security Group die Regeln. Wenn die Person erlaubt ist, wird der Zugriff gewährt. Wenn die Person nicht auf der Liste steht, wird der Zugriff verweigert.

Security Groups helfen dabei, deine Ressourcen in der Cloud vor unbefugtem Zugriff zu schützen. Sie sorgen dafür, dass nur diejenigen, die erlaubt sind, auf deine Daten und Dienste zugreifen können. Ähnlich wie ein Sicherheitsdienst auf deiner Party schützt die Security Group deine Ressourcen und sorgt für ein sicheres Umfeld.