---
share: true  
--- 
## YAML
YAML (YAML Ain't Markup Language) ist eine einfache, menschenlesbare Datenstruktursprache. Es wird oft als Dateiformat für die Konfiguration von Anwendungen und die Übertragung von Daten verwendet. YAML-Dateien verwenden eine textbasierte Syntax, die darauf abzielt, einfach zu sein und leicht verstanden zu werden. YAML kann verwendet werden, um komplexe Datenstrukturen wie Listen, Objekte und verschachtelte Hierarchien darzustellen. Es ist besonders nützlich für Konfigurationsdateien in Anwendungen oder für den Austausch von Daten zwischen verschiedenen Systemen.

### Beispiel
Hier ist ein einfaches Beispiel für YAML, das eine Konfigurationsdatei für eine Anwendung darstellt:

```yaml
# Konfigurationsdatei für eine Anwendung

app:
  name: Mein Beispiel-App
  version: 1.0.0
  environment: production

database:
  host: localhost
  port: 5432
  username: myuser
  password: mypassword
  dbname: mydatabase

server:
  host: 0.0.0.0
  port: 8080
```

In diesem Beispiel gibt es drei Hauptbereiche: `app`, `database` und `server`. Unter jedem Bereich sind Schlüssel-Wert-Paare aufgeführt, die verschiedene Einstellungen für die entsprechenden Komponenten darstellen.

Die `app`-Sektion enthält Informationen über den Namen, die Version und die Umgebung der Anwendung.

Die `database`-Sektion enthält Konfigurationsdetails für die Datenbankverbindung, wie den Host, den Port, den Benutzernamen, das Passwort und den Datenbanknamen.

Die `server`-Sektion enthält Konfigurationseinstellungen für den Webserver, wie den Host und den Port, auf dem die Anwendung ausgeführt werden soll.

Diese YAML-Konfigurationsdatei kann von der Anwendung eingelesen werden, um die entsprechenden Einstellungen zu laden und die Anwendung entsprechend zu konfigurieren. YAML bietet eine einfache und lesbare Syntax, um Datenstrukturen zu definieren und zu organisieren.