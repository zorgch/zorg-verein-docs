# Protokoll zorg Vorstandssitzung und Coding/neuer Server

Teilnehmer: Oliver Raduner, Nico Raschle, Dominik Angehrn, Florian Bentele

Wo: Hangouts

Wann: 18.02.2020, 21:00 - 21:45

## Themen zum neuen Server (Oli, Nico, Domi, Flo)
### PHP7 Upgrade
- Nur noch PHP7 auf neuem Server. PHP5 wird nicht mehr installiert.

### Neuer Server
- Neue Construct / Testumgebung auf neuem Server. Parallelbetrieb mit Produktivsystem möglich.
  - Testen im Construct. Bugs sammeln, beheben. Dann zorg auf neuen Server umziehen.
- Wie soll neuer Server heissen?
  - TODO (Oli): Voting aufsetzen
- Flo an Ubuntu Update dran. Testumgebung & Deployment-Skripts inkl. Deploy UI (Webpage) eingerichtet.
  - TODO (Flo): update Apache Configs im entsprechenden [Git Repository](https://github.com/zorgch/xoli-apache-configs)
  - TODO (Flo): erstellt User auf neuem Server für Vorstandsmitglieder.
  - TODO (Flo): Prüfen ob User inkl. PW & Userhomes vom xoli migriert werden können
  - TODO (Oli): sendet Info an bestehende xoli-User bzgl. Serverumzug.

### Security / Passwort Manager
- Angriffe / SQL-injections: Standard Apache rules könnten 90% abfangen.
  - TODO (Flo): prüfen ob aktuelle User-Passwörter in der DB genügend stark verschlüsselt sind.
  - TODO (Flo): installieren der Apache mod_security mit Standardconfigs.
  - Im Testing dann Inputs geben, wenn irgendwas nicht mehr funktioniert.
- Wo werden Passwörter (zentral) abgelegt? Gibts Konzept?
  - Diverse shared User (phpadmin, ...).
  - Bisher hat man sich selbst Berechtigung gegeben. Root brauchts nicht (`sudo` verwenden, wer berechtigt ist).
  - phpmyadmin konnte man früher auch mit eigenem User. Mittlerweile mit mysql workbatch. Aber phpMyAdmin trotzdem nützlich.
  - Vorschlag: Keepass-DB auf Server ablegen.
    - TODO (Oli): Keepass-Vault mit Masterpasswort auf xoli testen, Info an alle ob das funktioniert

### IRC
- Wir verwenden [ircd-hybrid mit anope services](https://linoxide.com/ubuntu-how-to/howto-setup-ircd-hybrid-anope-services-ssl-ubuntu/). Mehrheitlich standard Configs.
- TODO (Nico): schaut sich das an und dokumentiert das notwendige für Setup auf neuem Server

## Vorstandsthemen (Oli, Nico, Domi)
- Oli hat PPT Vorlage erstellt (mit schwarzem Hintergrund).
  - TODO (Oli): merge der neuen Vorlagen ins [Verein Git Repository](https://github.com/zorgch/zorg-verein-docs) (unter Hagwar CI/CD)
- Beitrittsformular für GangsterTi aufgesetzt
  - TODO (Oli): sendet Beitrittsformulat an Ti sobald Adresse bekannt.
- TODO (Oli): zorg UserIds, UserNames und Emailadresse von den 3 neuen Vereinsmitgliedern an Domi schicken für Update in der Mitgliederliste.
