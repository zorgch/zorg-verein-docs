* [Einleitung](#markdown-header-einleitung)
* [Neuerungen](#markdown-header-neuerungen)
  * [Wieso Markdown, nicht mehr TeX?](#markdown-header-wieso-markdown-nicht-mehr-tex)
  * [Wieso ein Git-Repository bei BitBucket?](#markdown-header-wieso-ein-git-repository-bei-bitbucket)
* [Feedback](#markdown-header-feedback-anregungen-oder-sonstige-anliegen)

# Einleitung

Liebe Mitglieder, liebe Freunde des Zorg Vereins, liebe Interessierte

Seit Gründung unseres Vereins hat der Vorstand stets darauf geachtet, dass alle wichtigen Dokumente, welche im Rahmen der offiziellen Vereinsaktivitäten erzeugt werden, in einem Format mit einer voraussichtlich möglichst langfristigen Lebensdauer erstellt werden. So stellen wir einen Plattform- und Software-unabhängigen Zugriff auf die Rohdaten sicher, der hoffentlich die Generationenwechsel in der sich verändernden IT-Landschaft überdauert, sowie auch bei allfälligen Wechsel von Vorstandsmitgliedern nicht zu einem "lock-in" führt.

Nebst dieser – sehr einfach zu lösenden – Herausforderung, haben wir aber auch den Anspruch, zentral, gemeinsam und stets auf die aktuellsten Versionen von Dokumenten zugreifen zu können. Zusätzlich ist es für den Einzelnen mit nicht unwesentlicher, manueller Arbeit verbunden, einen Änderungsverlauf über verschiedenste Dokumente zu führen – und zu schnell geht dabei trotzdem etwas vergessen.

# Neuerungen

Aus diesem Grund hat sich der Vorstand entschieden, dass wir alle für den Vorstand wichtigen und für die Vereinsmitglieder ebenso wissenswerte Dokumente neu in unserem Git-Repository führen werden. Dieser Schritt bringt folgende weitere Änderungen und Vorteile:

  1. Die Vereinsdokumente liegen am gleichen Ort, wie der Zorg Code
  2. Die Git-Repositories von BitBucket sind Cloud-basiert, sprich Zugriff auf die Informationen durch alle Mitglieder ist entsprechend sichergestellt - sowie die Einbindung z.B. auf [zorg.ch](https://zorg.ch/)
  3. Verwendung des [Markdown-Standards](https://en.wikipedia.org/wiki/Markdown) anstatt [TeX](https://en.wikipedia.org/wiki/TeX)
  4. Umfassende, automatisierte Versionierung sowie granularer Änderungsverlauf für jedes Dokument - gepaart mit Features wit "Branches" und "Tags" noch mächtiger
  5. BitBucket setzt auf Standards wie Git und Mercurial auf, ebenso auch mit Markdown-Unterstützung. Daher liesse sich dieser Software-Stack auch auf einem eigenen Server betreiben - Migrationsfähigkeit ist somit sichergestellt

## Wieso Markdown, nicht mehr TeX?
Da der Markdown-Syntax eigentlich Plain-Text ist, angereichert mit sehr wenigen, ebenfalls aber einfache Plain-Text Anweisungen, können Dokumente in diesem Format im schlimmsten Falle einfach unformatiert gelesen und bearbeitet werden.

TeX basiert grundsätzlich auf dem gleichen Ansatz, allerdings ist dieses so mächtig, dass es folgende Nachteile hat:

1. TeX-Programme und Suiten müssen Plattformabhängig beschafft und installiert werden, diese OpenSource Projekte hängen teilweise OS Updates (stark) hinten nach
2. je nachdem welche Anweisungen in einem TeX Dokument verwendet wurden, sind dazu viele zusätzliche TeX-Libraries notwendig, um ein TeX-Dokument wieder korrekt interpretieren zu können
2. die teils sehr komplexen Anweisungen machen ein TeX-Dokument im Plain-Text Modus schwieriger lesbar als Markdown
3. TeX kann standardmässig nur in PDF kompiliert werden, keine anderen Formate.


## Wieso ein Git-Repository bei BitBucket?
BitBucket ermöglicht uns – bis anhin kostenlos – mehrere Repositories zu erstellen und verwalten. Wie erwähnt, haben wir z.B. den Quelltext von [zorg.ch](https://zorg.ch/) schon länger hier und sehr gute Erfahrungen damit gemacht.

Grundsätzlich – ob BitBucket, GitHub, oder eine eigene Git-Umgebung – sind die Vorteile, nebst bereits aufgezähltem, dass quasi jeder sich auch an den Inhalten beteiligen kann:

Seien dies einfach Kommentare zu Dokumenten hier in der Ablage, oder spezifischen Stellen innerhalb eines Dokumentes – bis zu komplett umfassenden Änderungen oder neuen Inhalten: jeder Benutzer mit Zugriff auf das Zorg Verein Docs-Repository kann (mit etwas Git-Knowhow ;)) alle Files auschecken, bearbeiten, ergänzen und zurückspielen. Oder dies im Falle von Markdown-Dokumenten sogar gleich live und direkt im Webbrowser erledigen!

# Feedback, Anregungen oder sonstige Anliegen?
Meldet euch einfach beim Vorstand, einem Vorstandsmitglied, dem Serveradministrator – oder noch einfacher: nutzt das [Zorg Forum](https://zorg.ch/forum.php) oder bringt direkt hier eure Kommentare ein!
