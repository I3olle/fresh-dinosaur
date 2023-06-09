---
share: true
---

## Was Ist IaC?

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

### Beispiel

Hier ist ein einfaches Beispiel für Terraform, um eine AWS EC2-Instanz zu erstellen:

```terraform
# Provider konfigurieren (AWS)
provider "aws" {
  region = "us-west-2"
}

# EC2-Instanz erstellen
resource "aws_instance" "example" {
  ami           = "ami-0c94855ba95c71c99"
  instance_type = "t2.micro"
}

# Ausgabe der erstellten Instanz
output "instance_ip" {
  value = aws_instance.example.public_ip
}
```

In diesem Beispiel wird eine AWS EC2-Instanz mit der angegebenen AMI (Amazon Machine Image) und Instanztyp erstellt. Das `provider`-Block definiert die AWS-Region, in der die Instanz erstellt werden soll.

Die `resource`-Block definiert die AWS-Instanz mit dem Namen "example". Sie verwendet die angegebene AMI und den Instanztyp, um die Instanz zu konfigurieren.

Der `output`-Block gibt die öffentliche IP-Adresse der erstellten Instanz aus.

### Provider

Ein Terraform Provider ist ein Plugin, das Terraform ermöglicht, mit einer spezifischen [API](../Begriffe/Netzwerk/Unsortiert.md#api) oder einem spezifischen Service zu interagieren. Jeder Provider fügt Terraform eine Reihe von Ressourcentypen hinzu, die es erstellen und verwalten kann.

Zum Beispiel könnte ein AWS Provider es Ihnen ermöglichen, EC2-Instanzen, S3-Buckets, RDS-Datenbanken und andere AWS-Ressourcen zu erstellen und zu verwalten. Ein Google Cloud Platform Provider könnte es Ihnen ermöglichen, Compute-Instanzen, Cloud Storage-Buckets, SQL-Datenbanken und andere GCP-Ressourcen zu erstellen und zu verwalten.

Es gibt Terraform Provider für eine Vielzahl von öffentlichen Clouds, private Clouds, SaaS-Anwendungen und andere Dienste. In vielen Fällen werden diese Provider von den Unternehmen selbst oder von der Open-Source-Community gepflegt und aktualisiert.

Mit diesen Providern kann Terraform als eine Art universelle "Sprache" für die Infrastrukturverwaltung dienen, die es Ihnen ermöglicht, Ressourcen in vielen verschiedenen Umgebungen mit einer einheitlichen, konsistenten Syntax zu verwalten.