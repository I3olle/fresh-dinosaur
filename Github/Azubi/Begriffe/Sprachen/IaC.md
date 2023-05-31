---
share: true  
--- 
# IaC

## IaC
IaC steht für Infrastructure-as-Code und bezieht sich auf den Ansatz, die Infrastruktur eines Systems mithilfe von Code zu definieren und zu verwalten. Anstatt die Infrastruktur manuell zu konfigurieren, können Entwickler mit IaC-Tools wie Terraform eine deklarative Konfigurationssprache verwenden, um Ressourcen wie Server, Netzwerkkomponenten und Cloud-Services zu beschreiben. Diese Beschreibungen werden dann verwendet, um die Infrastruktur automatisch bereitzustellen, zu verändern und zu löschen.

## Terraform
Terraform ist ein sogenanntes Infrastructure-as-Code (IaC)-Werkzeug. Es ermöglicht Entwicklern und Systemadministratoren, die Infrastruktur für ihre Anwendungen und Systeme über eine Codebasis zu verwalten.

Terraform ermöglicht es Entwicklern, Infrastrukturressourcen über verschiedene Cloud-Anbieter hinweg zu verwalten, darunter auch große Cloud-Plattformen wie Amazon Web Services (AWS), Microsoft Azure, Google Cloud Platform (GCP) und viele andere. Es bietet eine einheitliche Schnittstelle und Abstraktionsschicht, um Infrastrukturkonfigurationen plattformübergreifend und wiederverwendbar zu machen.

Mit Terraform können Entwickler ihre Infrastruktur in Form von Code versionieren, sodass Änderungen und Updates verfolgt und verwaltet werden können. Dadurch wird die Infrastrukturverwaltung konsistent, skalierbar und reproduzierbar. Terraform ermöglicht auch die automatische Skalierung und das dynamische Hinzufügen oder Entfernen von Ressourcen basierend auf Anforderungen oder Last.

Zusammenfassend ist Terraform ein IaC-Tool, das es Entwicklern ermöglicht, die Infrastruktur ihrer Anwendungen und Systeme über Code zu verwalten. Es bietet eine plattformübergreifende Schnittstelle zur Bereitstellung, Veränderung und Löschung von Infrastrukturressourcen in verschiedenen Cloud-Umgebungen. Dies erleichtert die Automatisierung, Skalierung und Wiederholbarkeit der Infrastrukturverwaltung.

### ELI5
Stell dir vor, du baust ein Lego-Set zusammen. Du hast viele verschiedene Lego-Steine und möchtest sie zu einem bestimmten Modell zusammensetzen. Aber statt jedes Mal von vorne anzufangen, wenn du das Modell ändern möchtest, verwendest du eine Anleitung, die dir sagt, welche Steine du wo platzieren sollst. 

Terraform ist wie diese Anleitung, aber für die Erstellung von Computer-Infrastruktur. Anstatt die Infrastruktur manuell Schritt für Schritt aufzubauen, kannst du Terraform verwenden, um eine Anleitung zu erstellen, wie deine Infrastruktur aussehen soll. 

Du beschreibst deine gewünschte Infrastruktur in einer speziellen Sprache, ähnlich wie eine Liste der benötigten Lego-Steine und wie sie zusammengebaut werden sollen. Terraform verwendet dann diese Anleitung, um die Infrastruktur automatisch zu erstellen, zu ändern oder sogar zu löschen.

Terraform unterstützt verschiedene Cloud-Plattformen wie Amazon Web Services (AWS), Microsoft Azure oder Google Cloud Platform (GCP). Es kennt die richtigen Schritte und die Reihenfolge, um die entsprechenden Ressourcen in der Cloud zu erstellen, wie Server, Netzwerke oder Datenbanken.

Wenn du Änderungen an deiner Infrastruktur vornehmen möchtest, änderst du einfach die Anleitung in Terraform. Es überprüft dann, welche Teile aktualisiert werden müssen und passt die Infrastruktur entsprechend an. So kannst du deine Infrastruktur einfach verwalten, ohne alles von Grund auf neu zu erstellen.

Zusammengefasst ist Terraform wie eine Anleitung, die dir sagt, wie du deine Computer-Infrastruktur aufbauen kannst. Du beschreibst, was du brauchst, und Terraform sorgt dafür, dass die Infrastruktur automatisch erstellt wird. Es hilft dir, Zeit zu sparen und deine Infrastruktur effizient zu verwalten, ähnlich wie beim Zusammenbauen eines Lego-Sets mit einer Anleitung.