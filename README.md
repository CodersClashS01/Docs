<div align="center">
  <img src="https://zekro.de/src/cclogo.png" width="300" >
  <h1>~ CodersClash ~</h1>
  <strong>Discord Bot Coding Tournament</strong><br><br>
  <a href="https://goo.gl/forms/kIHETPs6ObfjYs7J2">
    <img src="https://img.shields.io/badge/Team%20Anmdeldung-HIER-green.svg?longCache=true&style=for-the-badge" />
  </a><br>
  Sponsored by<br>
  <a href="https://signaltransmitter.de/ref/1f6r1028r25ef6550" >
    <img src="https://signaltransmitter.de/web/st-img/st_banner_300x50.gif"/>
  </a>
</div>
 
---

> `v.1.1` - `19.06.2018`

---

## Index

1. [Einleitung](#einleitung)
2. [Ablauf](#ablauf)
3. [Regeln](#regeln)
4. [Die Anforderungen](#die-anforderungen)
5. [Preise](#preise)
6. [Punktesystem](#punktesystem)
7. [Anmeldung](#anmeldung)

---

# Einleitung

Wir, das Staff-Team von zekro's Dev-Server, wollen gemeinsam mit euch ein kleines Tournament veranstalten, bei dem 2 oder mehr Teams einen Discord Bot erstellen sollen, welche dann in einer Testphase von den Membern des Servers bewertet werden können. Zu gewinnen wird es dabei natürlich auch etwas geben, jedoch soll es bei dem Turnier primär um den Spaß an der Sache gehen. ;)

---

# Ablauf

### Phase 1: Teamfindung
Zuerst werden sich Teams aus **mindestens 2 und maximal 5** Leuten bilden. Ihr könnt euch dann **[hier](https://goo.gl/forms/kIHETPs6ObfjYs7J2)** als Team anmelden.
> Diese Phase wird vom **18. Juni 2018** zum **22. Juni 2018** **(1 Woche)** andauern.

### Phase 2: Entwicklungsphase
In dieser Phase entwickeln die Teams die geforderten Features der Bots, welche vorher zufällig aus einer Liste von Features *(z.B. XP-System, Autorole, Voting-System, ...)* ausgewählt werden und für alle Teams gleich gelten. Während der Entwicklungsphase sollten die Repositories natürlich Closed Source sein.
> Diese Phase wird vom **23. Juni 2018** zum **21. Juli 2018** **(4 Wochen)** andauern.

### Phase 3: Testphase
In dieser Phase werden die Bots an das Test-Team übergeben. Das heißt, die Bots werden auf einem extra Server installiert und gehostet. Dann werden die Bots auf dem Dev-Discord veröffentlicht und allen Nutzern zur Verfügung gestellt. Zudem werden ab dann die Repositories der Bots auf GitHub veröffentlicht und verschiedenen Tests unterzogen, welche unten detailliert genannt werden.
> Diese Phase wird vom **22. Juli 2018** zum **12. August 2018** **(3 Wochen)** andauern.

### Phase 4: Votingphase
In dieser Phase können alle Member des Servers abstimmen, welchen Bot sie am besten fanden. Test- und Auswertungsphase sind deswegen voneinander getrennt, da natürlich die Bots auch auf ihre Stabilität und ihr "Durchhaltevermögen" getestet werden sollen.
> Diese Phase wird vom **13. August 2018** zum **17. August 2018** **(1 Woche)** andauern.

Somit werden am **18. August 2018** die Ergebnisse veröffentlicht.

---

# Regeln

- Selbstverständlich müssen die Bots in den gegebenen Environments selbstständig und stabil laufen.
- Die Bots müssen auf Linux Debian laufen.
- Sollte ein Bot in der Testphase crashen wird dieser nur neu gestartet, wenn es sich dabei um einen Disconnect, Timeout oder sonst einen Fehler der Umgebung handeln sollte. Ansonsten ist ab dem Zeitpunkt des Crashes die Testphase für den Bot beendet, darf jedoch beim Voting noch Teilnehmen.
- Generell dürfen alle Packages der Languages und Wrapper benutz werden. Sollte ein Team unbedingt 3rd-Party-Libraries benötigen, so können diese in Absprache mit dem Discord-Staff-Team benutzt werden.
- Der Bot muss eine Konfigurationsdatei beinhalten, mit der Dinge wie Token, Prefix, Datenbankdaten und Botowner einstellbar sind.
- Die Bots müssen eine Dokumentation ihrer Commands mitbringen *(z.B. in Form einer Website, online PDF oder eines Gist auf GitHub bzw. in der Readme oder im Wiki der Repository)*.

### Das Testsystem

Der Testserver wird von **[signaltransmitter.de](https://signaltransmitter.de/ref/1f6r1028r25ef6550)** zur Verfügung gestellt.

| | |
|---|---|
| System    | debian-8.0-x86_64 |
| Type      | OpenVZ |
| RAM       | 4 GB |
| CPU       | 4 VCores |
| Anbindung | 250 MBit/s Up/Down |
| Software  | - MySql/MongoDB<br>- Java<br>- Go<br>- Rust<br>- Ruby / Gem<br>- Python / PIP<br>- NodeJs / NPM<br>- Jenkins<br>- git<br>- screen<br>- ServerManager2 |

### Erlaubte Dependencies und API Wrapper

Folgende API Wrapper stehen zur Auswahl:

Language | Library
---------|---------
Node.js  | discord.js<br>Eris<br>discordie
Java     | Discord4J<br>JDA<br>Javacord
Go       | discordgo
Python   | discord.py
Rust     | discord-rs<br>serenity
Ruby     | discordrb

Zudem sind Libraries um auf eine Datenbank zugreifen zu können erlaubt.

---

# Die Anforderungen

Die folgenden Anforderungen **muss** der Bot beinhalten:

- **Eine Config**  
  *In dieser der Token des Bots, der Owner, die Credentials zu API's und zu der Datenbank und weitere beliebige Einstellungen getätigt werden können.*
- **Command Parser und Event Handler**  
  *Selbstverständlich sollte der Bot die Grundbausteine nahezu aller Bots beinhalten, um funktionieren zu können.*
- **Datenbankanbindung an MySql oder MongoDB**  
  *Sollte für die Umsetzug der Features die Speicherung von Daten nötig sein so sollte dies über eine Datenbank erfolgen.*
- **Permission System**  
  *Natürlich muss es eine Verwaltung geben, welche Nutzer was machen können. Wie ganau dieses System umgesetzt ist ist Entscheidungssache des Teams.*

Aus folgender Liste werden dann zufällig **4** Anforderungen gezogen, welche die Bots beinhalten müssen.

- **XP-System** `Complex`  
  *Vergabe von XP-Punkten an User. Unter welchen Kriterien diese erfolgt und welche Belohnungen dabei ausgeschüttet werden ist Endscheidung des Teams.*
- **Music Command** `Complex`  
  *Einen umfangreichen Music-Command mit dem man von Online-Platformen wie z.B. YouTube Musik (auch in form von Playlists) streamen kann.*
- **Ein Game-Feature** `Complex`  
  *Es soll ein Chat-Game erstellt werden, welches User zusammen spielen können. Welches genau hängt von der Kreativität des Teams ab. ;)*
- **Message-Filter** `Complex`  
  *Filtern von Messages auf unerlaubte Links, Schimpfworte, ...*
- **Voting System** `Medium`  
  *Ein System, mit dem User Votes erstellen können und unter diesen Abstimmen können.*
- **Autochannel-System** `Medium`  
  *Automatisches erstellen von teporären Voice-Channels beim Joinen des Root-Channels (z.B. wie beim RubiconBot oder zekroBot2).*
- **Report-System** `Medium`  
  *Reporting von Usern und aufzeichnung in Datenbank.* 

Zudem soll jeder Bot mindestens **2** weitere, **inovative** Features haben. Um was es sich dabei handelt ist vollkommen den Teams überlassen, es sollte jedoch etwas sein, was man bis jetzt noch nicht gesehen hat.

Natürlich können auch noch weitere dinge in den Bot implementiert werden, welche hier nicht aufgelistet sind. Es geht ja schließlich auch um das Gesamtbild des Projekts. ;)

---

# Punktesystem

| | | |
|---|---|---|
| codacy | - A<br>- B<br>- C<br>- D<br>- E<br>- F | `+ 150 P`<br>`+ 100 P`<br>`+ 50 P`<br>`+ 10 P`<br>`0 P`<br>`0 P` |
| User Voting | Anteil der Stimmen des Bots multipliziert mit 1000 Punkten. | `Bot-Stimmen / Gesamtstimmen * 1000 P` |
| Staff Voting | Anteil der Stimmen des Bots multipliziert mit 300 Punkten. | `Bot-Stimmen / Gesamtstimmen * 350 P` |
| Bot-Crash während Testphase | | `- 500 P` |
| Bot startet nicht auf Test-System | Disqualifikation | |
| **Gesamtzahl erreichbarer Punkte** | | **`1500 P`** |

---

# Preise

Wie schon gesagt soll es bei dem Event nicht um einen großen Preis gehen, sondern eher um den Spaß und die Ehre. Jedoch gibt's natürlich trotzdem ein paar Goodies für die Gewinner:

- Alle Teilnehmer des Gewinnerteams bekommen die seperat angezeigte Rolle **`CodersClash S01 Gewinner`**
- Der Gewinner-Bot bekommt zudem eine extra Bot-Rolle mit erweiterten Rechten  
  *Dabei ist zu beachten, dass der Bot entweder kostenlos vom Server-Team gehostet werden kann oder von den Erstellern selbst unter der Bedigung, dass das Admin-Team Zugriff auf den Server und den Bot hat.*
- Zudem wird der Bot in einem seperaten Video auf zekro's YouTube-Kanal vorgestellt

---

# Anmeldung

[**Anmeldung**](https://goo.gl/forms/kIHETPs6ObfjYs7J2)
