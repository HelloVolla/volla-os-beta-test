# Volla OS Leitfaden

Das Betriebssystem Volla OS und dessen spezielle Benutzeroberfläche wird kontinuierlich weiterentwickelt. Einen Überblick über den Entwicklungsstand finden Sie auf der Plattform Github, auf wir dem Quellcode des Betriebssystems veröffentlichen. 

https://github.com/HelloVolla/

In dem Repositorium [volla-os-beta-test](https://github.com/HelloVolla/volla-os-beta-test) finden Sie neben dieser Anleitung auch die Möglichkeit Fehler zu melden und deren Behebung zu verfolgen. 

https://github.com/HelloVolla/volla-os-beta-test/issues

Wenn Sie ein Volla Phone mit einem Volla OS Betriebssystem entsperren, gelangen Sie zum Volla Launcher, den Sie die Grundfunktionen des Gerätes einschließlich das Öffnen von Apps ausführen können. 

Sie erreichen den Volla Launcher auch durch die Home Schaltfläche an der unteren Seite der Anzeige oder durch die entsprechende Wischgeste von der unteren Außenseite der Anzeige in den Innenbereich.

Das vollständige Ausblenden der Android Navigationsleiste erfolgt für den Volla Launcher in dessen Einstellungen in der Gruppe „Anzeige und Menüs“ durch Tippen auf „Vollbildansicht“. Sie gelangen zu den Einstellungen des Volla Launchers, indem Sie zweimal nach rechts wischen, sodass von der linken Seite die Einstellungen erscheinen.

Die Volla Benutzeroberfläche umfasst zwei Grundkonzepte:

1. Sprungbrett mit
	2. Textfeld und
	3. Kurzbefehlen
3. Sammlungen für
	4. Kontakte
	5. Unterhaltungen
	6. Nachrichten
	7. Notizen

## Sprungbrett

Immer wenn Sie den Volla Launcher aufrufen, zeigt dieser das Sprungbrett. Die Idee ist, dass Sie etwas schreiben und das System erkennt, was Sie zum wollen. Dafür liefert es Vorschläge zur Vervollständigung Ihrer Eingabe oder passende Funktionen für Ihre Eingabe.

![Springboard](screenshot-springboard.jpeg)

Das Sprungbrett unterstützt folgende Anwendungsfälle:

### Kontaktauswahl
Wenn Sie die Eingabe mit dem @-Zeichen beginnen, erkenn das System, dass Sie einen Namen eingeben wollen und schlägt Personen aus em Adressbuch vor, die vorläufig nach Namen sortiert sind. Tippen Sie auf einen Namen in der List, wird dieser im Textfeld übernommen. Voraussetzung für diese Funkton ist, dass sich In Ihrem Adressbuch Einträge befinden.

Durch die Eingabe weiterer Buchstaben können Sie die Liste der Kontakte filtern. Hierbei zeigt das Sprungbrett die Namen an, die die eingegebene Buchstabenfolge an beliebiger Stelle enthalten.

Sie können Kontakt beispielsweise mit der installierten App für die Synchronisation von Adressbüchern und Kalender über das CardDAV und CalDAV Protokoll synchronisieren.

### Anruf
Anschließend schlägt das System vor, dass Sie diese Person anrufen. Wenn Sie auf den Vorschlag für diese Funktion tippen, startet das System einen Anruf über die Telefonie-App. Vorschläge für Funktionen erkennen Sie im Unterschied zu Vorschlägen zur Vervollständigung Ihrer Eingabe and der roten Hintergrundfarbe.

	@Claudia_Sommer

### Mitteilungen
Wenn Sie anstatt einen Anruf auszulösen weitere Worte eingeben, schlägt das System vorn, dass Sie dem eingegebenen Kontakt eine Kurzmitteilung oder E-Mail senden können. Tippen Sie auf den Vorschlag öffnet die App aktuell noch die jeweilige App mit eine vorausgefüllten Mitteilung, die Sie nur noch absenden müssen. 

	@Claudia Sommer Kommst Du mit uns zum Italiener in der Mittagspause?

Verwenden Sie einen Zeilenumbruch nach den Worten, verwendet das System die erste Zeile für den Betreff einer E-Mail. Voraussetzung ist, dass Sie mindestens ei E-Mail-Konto angelegt haben.

	@Claudia_Sommer Mittagspause
	Hast Du Lust in der Mittagspause mit uns zum Italiener zu gehen?\
	Grüße von Petra
	
In Abhängigkeit der für einen Kontakt hinterlegten Daten, schlägt der Volla Launcher vor, eine Nachricht als SMS, E-Mail über den Signal Messenger Dienst zu versenden.  

### Web-Suche
Wenn Sie die Eingabe anstatt mit einem Wort anstatt eines Kontaktes starten, schlagt das System vor, mit diesem Wort im Internet zu suchen. Dafür startet das System den Browser mit dem eingegebenen Stichwort. Als Standard verwendet der Volla Launcher die Suchmaschine [DuckDuckGo](https://duck.com). In den Einstellungen können Sie in der Gruppe „Suchmaschinen“ auch [Starpage](https://startpage.com) oder [Metager](https://metager.de) auswählen.

	Volla
	
### Notiz
Geben Sie mehrere Worte ein, schlägt das System außerdem vor, dass Sie eine Notiz anlegen können. Diese finden Sie anschließen als einen Eintrag in der Sammlungen für Notizen über den roten Punkt wieder.

	Volla Phone
	
Sie können auch Zeilenumbrüche verwenden.

	Volla Phone
	Neue Funktionen:
	1. Sichrheitsmodus
	2. Mult Boot
	
### Web-Adresse
Wenn Sie eine gültige Internetadresse eingeben, schlägt das System vor, diese im Browser zu öffnen.

	volla.online
	
### Telefonnummer
Wenn Sie das Textfeld eine Telefonnummer eingeben, schlägt Ihnen auch hier Das system vor, einen Anruf auszulösen. Wie bei allen Eingaben ist ein Leerzeichen am Ende eines Wortes oder eine Ziffernfolge notwendig um die Auswertung der Eingabe anzustoßen.

	014323566777
	
Geben Sie anschließend ein oder mehrere Worte ein, bietet das System an, dass Sie eine Kurzmitteilung senden, nicht jedoch eine E-Mail.

	014323565777 Hallo Petra, wie geht es Dir?
	
### E-Mail-Adresse

Wenn Sie eine E-Mail-Adresse und einen Text eingeben, schlägt der Volla Launcher das versenden einer E-Mail vor. 

	hello@volla.online Where can I buy a Volla Phone?  
	
Wenn Sie mehrere Zeiten eingeben, wird die erste Zeile als Betreff der E-Mail verwendet:
	
	hello@volla.online Volla retailer
	Dear Volla team,
	Where can I buy a Volla Phone? 	

### Kalenderereignis

Der Volla Launcher erkennt verschiedene Formen der Beschreibung eines Kalenderereignisses, das aus Datum, optionale Uhrzeit, Titel und optionale Beschreibung besteht. 

	12.08.2022 12 Uhr Mittagessen mit Peter
	12.08. 16:30 - 17:30 Training im Sportverein
	6 - 8 pm Abendessen mit Paula in Joe's Pizzaria  

Fehlt die Uhrzeit plant der Volla Launcher ein Tagesereignis. Fehler nur die zweite Uhrzeit für das Ereignis ein. Fehlt das Datum gilt der gleiche Tag. 

An Stelle eines Datums können Sie auch Wochentage oder eine Kurzform wählen:

	Morgen 10 Uhr Videokonferenz mit Paula
	Donnerstag 14 - 18 Uhr Weinseminar im Ratskeller 

Bei einem Zeilenumbruch verwendet der Volla Launcher den Text nach dem ersten Zeilenumbruch als Beschreibung des Kalenderereignisses. 

Wenn Sie auf den Vorschlag tippen, den Termin in den Kalender einzutragen, öffnet das System die Kalender App, in der Sie das Ereignis bestätigen, um es abzuspeicerh.
	
Weitere Anwendungsfälle sind geplant.

## Kurzbefehle

Auf dem Sprungbrett ist auf ein roter Punkt zu sehen. Mit diem rufen Sie Kurzbefehle mit nur einer Geste auf. Berühren Sie dafür den Punkt, sodass sich das Menü öffnet, schieben Sie den Finger oder Stylus über den gewünschten Menüeintrag und heben Sie den Finger oder Stylus an:

1. Berühren
2. Schieben
3. Loslassen

![Shortcuts](sceenshot-shortcuts.jpeg)

Der Standard enthält folgende Funktionen:

- Aufruf von jüngsten und favorisierten Kontakten
- Aufruf von jüngsten Konversationen
- Aufruf von jüngsten Nachrichten
- Aufruf von Notizen
- Aufruf der Telefon App
- Aufruf der Kamera
- Aufruf der Galerie
- Aufruf der Kalender App

Die Kurzbefehle können Sie in den Einstellungen unter der entsprechenden Gruppe des Volla Launchers verwalten. Standard-Funktionen können Sie deaktivieren und aktivieren, während Sie selbst definierte Kurzbefehle auch löschen können. 

Sie können auf zwei Wegen neue Kurzbefehle hinzufügen:

1. Tippen Sie auf eine App in der Übersicht und halten Sie die Berührung so lange bis ein Kontextmenü erscheint und wählen Sie die Option „Zu Kurzbefehlen hinzufügen“.
2. Wischen Sie vom Sprungbrett zwei mal nach rechts um von links die Einstellungen einzublenden. Tippen Sie auf die Gruppe „Kurzbefehle“ und anschließend auf das Plus-Zeichen, um ein Kontextmenü zu öffnen, über das Sie ine App auswählen können. 

Ein Tipp: Auch Internetadressen, die Sie als Lesezeichen in der App-Übersicht aufgenommen haben können Sie über diesen Weg zu den Kurzbefehlen hinzufügen. 

## Sammlungen

Die Sammlungen geben Ihnen einen schnellen Überblick über wichtige Informationen und passende Funktionen. Nach dem Aufruf einer Sammlung sehen Sie eine Animation, mit der das System die Sammlung von der rechten Seite einblendet.

Sie können mit eine Wischgeste, dem Home-Button oder der Home-Geste wieder zurück zum Sprungbrett navigieren. 

Jede Sammlung können Sie über ein Textfeld unter der Überschrift filtern.

### Kontakte
Das System stellt automatisch wichtige Kontakte zusammen. In der Beta-Version berücksichtig das System alle Kontakte, die Sie im Adressbuch als Favorit gekennzeichnet haben oder mit der Sie vor kurzem über einen Telefonanruf oder eine SMS oder MMS-Mitteilung in Verbindung standen.

In der Übersicht der Kontakte finden Sie den Namen des Kontaktes sowie dessen Organisation oder die jüngste ungelesene Nachricht oder ein verpasster Anruf. 

Tippen Sie auf einen Eintrag und halten Sie die Berührung eine kurze Zeit öffnet dass System ein Kontextmenü und bietet in Abhängigkeit, des Adressbucheintrags folgende Funktionen an: 

- Aufruf des Adressbucheintrags
- Aufruf des Signal-Profils
- Start eines Anrufs
- Aufruf der Messenger App zum Schreiben und Senden einer Kurzmitteilung
- Aufruf des E-Mail-App zum Schreiben und Senden eine E-Mail

Auch hier erfolgt die Auswahl gemäß der Geste für Kurzbefehle.

Tippen Sie nur kurz auf einen Eintrag, öffnet das System die Konversation mit der Person, die vorläufig Anrufe, SMS- und MMS-Mitteilungen enthält.

An der unteren Seite der Ansicht finden Sie ein Textfeld, über das Sie direkt per SMS oder MMS antworten können. 

In Vorbereitung ist eine Integration von Signal-Nachrichten. 

### Konversationen
Hier zeigt das System die jüngste Konversationen mit Name oder Telefonnummer und Text an, die es nach Zeit und Thema sortiert. Die Beta-Version berücksichtigt SMS- und MMS-Mitteilungen. Weitere Kommunikationskanäle sind geplant.

Tippen Sie kurz auf eine Konversation, zeigt das System die Konversation mit allen ausgetauschten Mitteilungen.

Auch hier können Sie über das Textfeld am unteren Rand direkt per SMS, MMS und in Zukunft über den Signal Messenger Dienst antworten

### Nachrichten
Hier zeigt das System die jüngsten Nachrichten nach ihrer Quelle gruppiert und nach Zeit sortiert. Das hat den Vorteil, dass wichtige Nachrichten aus Quellen, die seltener Nachrichten veröffentlichen nicht im Nachrichtenstrom untergehen. 

Wenn Sie auf das Symbol des Nachrichtenkanals tippen, gelangen Sie zu allen jüngsten Veröffentlichungen dieses ausgewählten Nachrichtenkanals. 

Tippen Sie hingegen auf die angezeigte Nachricht, gelangen Sie zu der vollständigen Nachricht, die das System für eine optimale Lesbarkeit aufbereitet.

Als Standard zeigt der Volla Launcher beispielhaft den RSS-Feed von drei Nachrichtenkanälen. Über zwei Wege können Sie eigene RSS oder Atom-Feeds von Nachrichtenportalen und Blogs abonnieren: 

1. Tippen Sie im Browser auf einen Link zu einem RSS- oder Atom-Nachrichten-Feed und halten Sie die Berührung so lange, bis ein Kontext-Menü erscheint. Wählen Sie die Option zum Teilen des Links mit dem Volla Launcher. 
2. Schreiben Sie den Link zu einem RSS- oder Atom-Nachrichten-Feed in das Textfeld des Sprungbretts oder kopieren Sie ihn hinein. Das Sprungbrett wird Ihnen vorschlagen, diesen Feed zu abonnieren. 

In den Einstellungen des Volla Launchers können Sie Nachrichten-Feeds in der Gruppe „Nachrichtenkanäle“ deaktivieren und aktivieren oder auch vollständig löschen, indem Sie auf das Kreuz am rechten Rand tippen. 

### Notizen
In dieser Sammlung führt der Volla Launcher alle Notizen auf, die Sie entweder über das Sprungbrett oder in der Listenansicht dieser Sammlung erstellt haben.

Tippen Sie auf einen Listeneintrag, um die vollständige Notiz zu lesen. In der Detailansicht können Sie eine Notiz bearbeiten, löschen oder an den Anfang der Liste anheften. Angeheftete Notizen können über den gleichen Weg auch wieder von der Position gelöst werden. 

Links mit oúnd ohne Protokoll-Präfix und Listen erkennt der Volla Launcher automatisch un formatiert diese auch automatisch.

	Eine Liste
	1, Sortierte Listen
	- Unsortierte Listen
	* Verschiedene aufzählungszeichen

## Apps

Wenn Sie vom Sprungbrett aus eine Wischgeste nach rechts ausführen gelangen Sie zur Übersicht der installierten Apps, die in alphabetischer Reihenfolge der Namen sortiert aufgeführt sind.

Als Standard sind die Apps in zwei Gruppen unterteilt: In häufig genutzte Apps und weitere Apps. Über die Einstellungen des Volla Launchers können Sie die Apps auch ungruppiert anzeigen lassen oder in weitere Gruppen, eine für jede App-Kategorie, anzeigen lassen. 

Unabhängig von der Gruppierung können Sie die angezeigten Apps über das Textfeld filtern.

Ein roter Punkt deutet an, ob Sie eine Anruf verpasst habe oder eine Kurzmitteilung och nicht gelesen haben.

## Einstellungen

Wenn Sie vom App-Gitter aus eine Wischgeste nach rechts ausführen gelangen Sie zu den Einstellungen der App. 

Als erste Gruppe finden Sie die Auswahl des Gestaltungsthemas. 

- Dunkler Modus
- Heller Modus
- Durchsichtiger Modus

Der durchsichtige Modus verwendet das Hintergrundbild, dass Sie in den Systemeinstellungen verändern können. Eine Änderung des Gestaltungsmodus definiert auch zugleich das Hintergrundbild des Sperrbildschirms. 

## Standard Apps

Das Volle OS kommt ohne Google Apps und Play Services, um die Privatsphäre der Anwender zu schützen. Daher enthält es kuratierte, quelloffene Alternativen. Siehe hierzu auch die entsprechende Übersicht. 

https://github.com/HelloVolla/volla-os-beta-test/wiki/Curated-Pre-Installed-System-Apps

Zu Auswahl ist noch nicht final. 

## Verschiedenes

Auch dieses Dokument wird überarbeitet werden. Allgemeine Fragen und Anregungen sind über unser Kontaktformular oder über die Volla Beta-Tester Gruppe auf Telegram willkommen:

https://volla.online/de/contact/

Für die Einladung in die Telegram Gruppe für die Beta-Tester, bitte Marc Aurel mit der Adresse @m_aurel anschreiben.