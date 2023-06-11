---
share: true
---

# Strukturierung

## Organizational Units:

Organisationseinheiten (auf Englisch "Organizational Units", abgekürzt OUs) sind ein Konzept aus der Verwaltung von Informationssystemen und werden oft in Verbindung mit Verzeichnisdiensten wie Microsoft's Active Directory (AD) oder dem Lightweight Directory Access Protocol (LDAP) verwendet.

Eine Organisationseinheit ist im Grunde ein Container innerhalb des Verzeichnisdienstes, in dem Benutzer, Gruppen, Computer und andere Organisationseinheiten organisiert und gruppiert werden können. Diese Strukturierung ermöglicht eine einfachere Verwaltung von Ressourcen und Richtlinien innerhalb einer Organisation.

Zum Beispiel könnte eine große Firma ihre Active Directory Struktur nach ihren Abteilungen organisieren, mit separaten Organisationseinheiten für die Personalabteilung, die IT-Abteilung, die Finanzabteilung und so weiter. Innerhalb jeder dieser Organisationseinheiten könnten dann Benutzer und Computer gruppiert werden, die spezifisch für diese Abteilung sind.

Diese Organisationseinheiten können dann dazu verwendet werden, Sicherheitsund Zugriffsrichtlinien zu verwalten. In unserem vorherigen Beispiel könnte die IT-Abteilung spezielle Zugriffsrechte auf bestimmte Systeme haben, die den Benutzern in den anderen Organisationseinheiten nicht gewährt werden. Durch die Anwendung dieser Richtlinien auf die Organisationseinheit anstatt auf jeden einzelnen Benutzer kann die Verwaltung solcher Zugriffsrechte erheblich vereinfacht werden.

### ELI5

"Organisationseinheiten" klingt ziemlich kompliziert, nicht wahr? Lass uns das vereinfachen.

Stell dir vor, du hast ein großes Spielzeughaus mit vielen verschiedenen Zimmern - es gibt ein Zimmer für die Küche, eines für das Wohnzimmer, eines für das Schlafzimmer und so weiter. In jedem Zimmer platzierst du verschiedene Spielzeuge, die zu diesem Raum passen - in der Küche befinden sich Spielzeugtöpfe und -pfannen, im Wohnzimmer ein Spielzeugfernseher und so weiter.

In einem großen Unternehmen mit vielen Computern und Benutzern funktioniert es ähnlich. "Organisationseinheiten" sind wie die Zimmer im Spielzeughaus. Sie helfen dabei, alles ordentlich zu organisieren. Zum Beispiel gibt es eine "Organisationseinheit" für die Buchhaltung, eine für das Marketing, eine für die IT-Abteilung und so weiter. In jeder dieser "Einheiten" befinden sich die Computer und Benutzer, die zu dieser Abteilung gehören.

Und genau wie du verschiedene Spielregeln für jedes Zimmer im Spielzeughaus haben könntest (zum Beispiel "In der Küche tun wir so, als ob wir kochen"), so kann das Unternehmen verschiedene Regeln für jede Organisationseinheit festlegen. Zum Beispiel könnte es Regeln geben, die besagen, dass nur Benutzer in der IT-Einheit Zugriff auf bestimmte Computerprogramme haben.

Das macht alles viel einfacher zu verwalten!

# Authentifizierung

## SSO

SSO steht für Single Sign-On und ist ein Authentifizierungsservice, der Benutzern erlaubt, mit nur einem Satz von Anmeldeinformationen auf mehrere Anwendungen zuzugreifen. Das bedeutet, dass ein Benutzer sich nur einmal anmelden muss, um auf mehrere verschiedene Dienste oder Anwendungen zugreifen zu können.

SSO bietet eine Reihe von Vorteilen sowohl für die Benutzer als auch für die IT-Abteilung:

- Benutzerfreundlichkeit:
	- Da Benutzer sich nur einmal anmelden müssen, um auf alle ihre Anwendungen zuzugreifen, spart SSO ihnen die Zeit und den Aufwand, sich mehrere Benutzernamen und Passwörter zu merken und einzugeben.
- Verbesserte Sicherheit:
	- SSO reduziert das Risiko von Angriffen auf Passwörter, da weniger Anmeldeinformationen im Umlauf sind. Darüber hinaus kann SSO mit zusätzlichen Sicherheitsmaßnahmen wie Zwei-Faktor-Authentifizierung und strengerer Passwortrichtlinie kombiniert werden.
- Vereinfachtes Management:
	- Für IT-Abteilungen kann SSO das Management von Benutzerkonten und Zugriffsrechten vereinfachen. Beispielsweise muss bei einem Mitarbeiterwechsel nur ein einziges Konto deaktiviert werden, um den Zugriff auf alle Anwendungen zu sperren.

Ein bekanntes Beispiel für SSO ist Google. Wenn Sie sich bei Ihrem Google-Konto anmelden, haben Sie automatisch Zugriff auf verschiedene Dienste wie Gmail, Google Docs, YouTube und Google Photos ohne weitere Anmeldungen.

Es gibt jedoch auch einige Nachteile oder Risiken bei der Verwendung von SSO. Ein Hauptanliegen ist, dass, wenn die Anmeldeinformationen eines Benutzers kompromittiert werden, der Angreifer potenziell Zugang zu allen Anwendungen und Diensten erhält, die der Benutzer verwendet. Dieses Risiko kann jedoch durch die Verwendung von zusätzlichen Sicherheitsmaßnahmen wie Zwei-Faktor-Authentifizierung gemildert werden.

## Zwei-Faktor-Authentifizierung

Die Zwei-Faktor-Authentifizierung (2FA) ist ein Sicherheitsverfahren, das eine zusätzliche Ebene der Überprüfung zur Identifizierung eines Benutzers hinzufügt. Sie basiert auf dem Prinzip, dass eine effektive Authentifizierung mindestens zwei von drei möglichen Authentifizierungsfaktoren erfordert: etwas, das man weiß (wie ein Passwort), etwas, das man hat (wie ein physischer Schlüssel oder ein Smartphone), oder etwas, das man ist (wie ein Fingerabdruck oder ein Gesichtsscan).

Hier sind einige gängige Beispiele für 2FA:

- **SMS-Codes**: Nachdem Sie Ihren Benutzernamen und Ihr Passwort eingegeben haben, sendet der Dienst eine SMS mit einem einmaligen Code an Ihr Handy. Sie müssen diesen Code eingeben, um den Anmeldevorgang abzuschließen.
- **Authenticator Apps**: Apps wie Google Authenticator oder Authy generieren zeitlich begrenzte Codes auf Ihrem Handy, die Sie eingeben müssen, um sich anzumelden.
- **Physische Sicherheitsschlüssel**: Ein Gerät, das Sie in den USB-Port Ihres Computers einstecken, das als zweiter Faktor dient. Um sich anzumelden, müssen Sie sowohl Ihr Passwort eingeben als auch den Schlüssel einstecken.
- **Biometrische Daten**: Fingerprint-Scanner auf Handys oder Gesichtserkennungstechnologien können als zweiter Faktor dienen.

Die Zwei-Faktor-Authentifizierung bietet erheblich mehr Sicherheit als die einfache Passwortauthentifizierung. Selbst wenn jemand Ihr Passwort kennt oder errät, können sie sich normalerweise nicht anmelden, ohne Zugang zum zweiten Faktor zu haben. Aus diesem Grund wird die Verwendung von 2FA für alle wichtigen Online-Konten dringend empfohlen.

### Tools

#### Okta

Okta ist ein führendes Unternehmen im Bereich der Identitätsund Zugriffsverwaltung. Sie bieten Cloud-basierte Softwarelösungen an, die Organisationen dabei unterstützen, die Identität und den Zugriff ihrer Mitarbeiter, Partner und Kunden zu verwalten.

Die Produkte und Dienstleistungen von Okta umfassen:

- **Single Sign-On (SSO)**:
	- Okta bietet eine SSO-Lösung, die es Benutzern ermöglicht, mit einer einzigen Anmeldung auf eine Vielzahl von Anwendungen zuzugreifen. Dies vereinfacht den Zugriff für Benutzer und kann die Sicherheit verbessern, indem weniger Passwörter im Umlauf sind.
- **Multi-Faktor-Authentifizierung (MFA)**:
	- Okta bietet MFA-Lösungen an, um die Sicherheit der Benutzerkonten zu erhöhen. Dies kann die Eingabe eines Codes umfassen, der an das Telefon des Benutzers gesendet wird, oder die Verwendung biometrischer Daten wie Fingerabdrücken.
- **API-Zugriffsmanagement**:
	- Okta ermöglicht es Entwicklern, die Identitätsüberprüfung in ihre Anwendungen und Dienste zu integrieren, indem es APIs und Entwicklertools bereitstellt.
- **Lebenszyklusmanagement**:
	- Okta unterstützt Organisationen dabei, die Konten ihrer Benutzer während ihres gesamten Lebenszyklus zu verwalten, von der Erstellung neuer Konten über die Änderung von Zugriffsrechten bis hin zur Deaktivierung von Konten, wenn ein Mitarbeiter das Unternehmen verlässt.

Okta zielt darauf ab, eine nahtlose und sichere Benutzererfahrung zu bieten, indem es den Zugriff auf Anwendungen und Dienste über Geräte und Standorte hinweg vereinfacht und gleichzeitig hohe Sicherheitsstandards aufrechterhält. Die Lösungen von Okta sind in vielen Branchen weit verbreitet, darunter Technologie, Bildung, Gesundheitswesen und Finanzen.