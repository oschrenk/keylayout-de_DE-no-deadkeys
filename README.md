# README #

Deutsche Tastaturlayout ohne die [Tottasten](http://de.wikipedia.org/wiki/Tottaste)

- ´, AKut
- `, Gravis
- ^, Zirkumflex

Da mit OS X Lion diakritische Zeichen einfach durch das Gedrückthalten des jeweiligen Buchstaben erzeugt werden, gewinne ich diese Tottasten lieber als Hotkeys und spare mir einige Tastenanschläge.

## Installation ##

Das Repository klonen

	git clone https://github.com/oschrenk/keylayout-de_DE-no-deadkeys.git
	cd keylayout-de_DE-no-deadkeys

Mein Haupt-Account ist nur Standard-Benutzer und hat daher keine Administrator-Rechte. Ich muss also vorher zu einem Adminstrator-Account wechseln um genügend Rechte zu haben um das Keyboard-Layout-Bundle in das entsprechende Systemverzeichnis zu kopieren. Falls dein Account Administrationsrechte hat kannst du dir also diesen Schritt ersparen (und das `exit` dann entsprechend auch).

	su admin

Kopiere das Bundle in das Systemverzeichnis

	sudo cp -r Deutsch\ -\ Ohne\ Tottasten.bundle /Library/Keyboard\ Layouts/

Die Shell des `admin` Accounts verlassen

	exit

Aus- und Einloggen um das Layout in _Systemeinstellungen > Sprache & Text > Eingabequellen_ sichtbar zu machen.

	$ osascript -e 'tell application "System Events" to log out'

# Danke!

Das Layout wurde mit Hilfe von [Ukulele](http://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&id=ukelele) erstellt.

