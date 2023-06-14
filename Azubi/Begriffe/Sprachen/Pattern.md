---
share: true
---

## Regular Expressions

Reguläre Ausdrücke, oft abgekürzt als RegEx oder RegExp, sind eine sehr mächtige Methode zur Mustererkennung in Text. Sie sind in vielen Programmiersprachen eingebaut und werden oft zur Textsuche, Textmanipulation und zum Parsen verwendet.

Eine reguläre Ausdruck ist im Grunde eine Sequenz von Zeichen, die ein Muster bildet. Dieses Muster kann verwendet werden, um Übereinstimmungen in anderen Strings zu finden oder zu testen.

### Komponenten

Hier sind einige grundlegende Komponenten, die in regulären Ausdrücken verwendet werden:

#### Literal-Zeichen

Die einfachsten Muster bestehen aus Literal-Zeichen, wie z. B. `abc`, das eine Übereinstimmung mit dem genauen String `abc` findet.

#### Metazeichen

Diese haben eine spezielle Bedeutung, z. B. `.` (findet jedes einzelne Zeichen außer einem Zeilenumbruch), `*` (findet null oder mehr Wiederholungen des vorhergehenden Zeichens), `+` (findet eine oder mehr Wiederholungen des vorhergehenden Zeichens) usw.

#### Charakterklassen

Sie stellen einen Satz von Zeichen dar, von denen jedes ein Treffer sein kann. Zum Beispiel steht `[abc]` für ein Zeichen, das entweder `a`, `b` oder `c` ist.

#### Quantifizierer

Diese bestimmen, wie oft ein Element wiederholt wird. Beispielsweise steht `{3}` für genau dreimal, `{3,}` für dreimal oder mehr, und `{3,5}` für zwischen drei und fünf Mal.

#### Anker

Diese werden verwendet, um den Anfang `^` oder das Ende `$` eines Strings oder einer Zeile zu bestimmen.

#### Gruppen Und Rückverweise

Zeichen können in Gruppen `()` eingefasst und später mit `\1`, `\2` usw. referenziert werden.

#### Escape-Sequenzen

Einige Zeichen müssen "escaped" werden, indem man ihnen ein `\` voranstellt, um sie wörtlich zu nehmen, z. B. `\.`, um einen tatsächlichen Punkt zu finden, anstatt jedes Zeichen.

### Beispiel

Hier ist ein Anwendungsfall für reguläre Ausdrücke (RegEx).

Angenommen, du hast eine Liste mit E-Mail-Adressen und du möchtest prüfen, ob sie ein gültiges Format haben. Eine einfache (aber nicht vollständig akkurate) RegEx zum Überprüfen des E-Mail-Formats könnte so aussehen:

```regex
^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$
```

Lass uns diesen regulären Ausdruck Stück für Stück durchgehen:

- `^` bezeichnet den Anfang der Zeile.
- `[a-zA-Z0-9._%+-]+` steht für einen oder mehr Buchstaben (Groß- oder Kleinbuchstaben), Ziffern, Punkte, Unterstriche, Prozentzeichen, Plus- oder Minuszeichen.
- `@` ist das @-Zeichen selbst.
- `[a-zA-Z0-9.-]+` steht wieder für einen oder mehr Buchstaben (Groß- oder Kleinbuchstaben), Ziffern, Punkte oder Bindestriche.
- `\.` ist ein Punkt.
- `[a-zA-Z]{2,}` steht für zwei oder mehr Buchstaben (Groß- oder Kleinbuchstaben).
- `$` bezeichnet das Ende der Zeile.

Dieser reguläre Ausdruck würde also auf Zeichenketten wie "example@example.com" passen, aber nicht auf "example@", da dies kein gültiges E-Mail-Format ist.

Bitte beachte, dass diese RegEx nicht alle gültigen E-Mail-Adressen korrekt erkennt und viele unzulässige als gültig markieren könnte. E-Mail-Adressen folgen einer ziemlich komplexen Spezifikation und es ist ziemlich schwierig, sie mit einer einfachen RegEx vollständig korrekt zu validieren.

Aber dieses Beispiel zeigt gut, wie man reguläre Ausdrücke zum Überprüfen von Textmustern verwenden kann.

### Zu Beachten

Es ist wichtig zu beachten, dass die genaue Syntax und die verfügbaren Funktionen von regulären Ausdrücken je nach Programmiersprache oder Tool variieren können.

Obwohl reguläre Ausdrücke sehr mächtig sind, können sie auch sehr komplex und schwer zu lesen sein, insbesondere für komplizierte Muster. Daher ist es oft hilfreich, sie sorgfältig zu dokumentieren und zu testen.

## Globbing

"Globbing" bezeichnet in der Informatik ein Verfahren zur Übereinstimmung mit bestimmten Zeichenmustern in Strings. Es wird oft in Unix-Shell-Umgebungen und in Programmiersprachen verwendet, die ähnliche Fähigkeiten haben.

Im Allgemeinen wird Globbing verwendet, um mehrere Dateinamen oder Ordner auf einmal zu spezifizieren, indem man spezielle Zeichen oder Wildcards verwendet. Hier sind die grundlegenden Wildcards und ihre Bedeutung im Kontext des Globbing:

- `*`: Dieser Platzhalter steht für eine beliebige Anzahl von beliebigen Zeichen. Zum Beispiel würde `*.txt` alle Dateien mit der Endung `.txt` im aktuellen Verzeichnis entsprechen.

- `?`: Dieser Platzhalter steht für genau ein beliebiges Zeichen. Zum Beispiel würde `?.txt` alle Dateien mit einem einzigen Zeichen vor der `.txt` Endung entsprechen.

- `[...]`: Dieser Ausdruck definiert eine Zeichenklasse. Zum Beispiel würde `[ab]*.txt` alle Dateien entsprechen, die mit `a` oder `b` beginnen und mit `.txt` enden.

Es ist zu beachten, dass das Verhalten des Globbing je nach Betriebssystem und Shell etwas variieren kann. Darüber hinaus bieten einige Shells erweiterte globbing Optionen, wie z.B. die Bash Shell in Unix, die Funktionen wie rekursive Übereinstimmungen (`**`) und Negationen (`!`) unterstützt.

Es ist auch wichtig zu beachten, dass, obwohl Globbing und reguläre Ausdrücke ähnlich erscheinen können, sie tatsächlich unterschiedliche Syntax und Funktionen haben. Insbesondere sind die Wildcards in Globbing-Patterns in der Regel weniger mächtig und flexibel als die äquivalenten Konstrukte in regulären Ausdrücken.

### Beispiel

Ein häufiger Anwendungsfall von Globbing ist die Suche nach Dateien in einem Betriebssystem über die Kommandozeile.

Nehmen wir an, du bist ein Entwickler und arbeitest an einem großen Projekt mit vielen JavaScript-Dateien. Du hast das Gefühl, dass du irgendwo einen Fehler gemacht hast, aber du erinnerst dich nicht mehr genau, in welcher Datei. Du weißt jedoch, dass die Zeile, die du suchst, den Text `console.log` enthält.

Um alle JavaScript-Dateien in deinem aktuellen Verzeichnis nach dieser Zeichenkette zu durchsuchen, könntest du in einer Unix-ähnlichen Shell folgenden Befehl verwenden:

```bash
grep 'console.log' *.js
```

In diesem Befehl steht `*.js` für "jede Datei, die mit `.js` endet". Das Sternchen (`*`) ist ein Beispiel für Globbing. Es fungiert als Platzhalter für "jeden Text".

Der Befehl `grep` durchsucht dann jede dieser Dateien nach der Zeichenkette `console.log` und gibt die entsprechenden Zeilen aus.

Das ist ein einfaches Beispiel, aber man kann sich leicht vorstellen, wie nützlich Globbing sein kann, wenn man mit vielen Dateien arbeitet und komplexe Muster suchen muss.