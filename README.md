## Inhalt
Dieses Repository enthält die Freifunk-Firmware, so wie sie im Freifunk-Netz in Frankfurt am Main (Ffm) verwendet wird. Es ist ein Fork der KBU-Firmware, die wie lff wiederum ein Fork der Lübecker Firmware ist.

## Branches
Die Branches im Upstream werden im gitweb aufgeführt: https://git.metameute.de/lff/firmware/ . In diesem Repository sind verfügbar:
+ master (README.md)
+ v0.3-generic
 
Andere Branches im Upstream sind nicht für die Verwendung für Freifunk-KBU angepasst (d.h. es gibt hierzu keine Kopie mit patches für abweichende Konfigurationen).
Der Generic-Branch enthält alle AR71xx-basierten Gerättypen.

## Checkout / Clone
Für einen build reicht ein checkout des Repositories aus. Hierzu muss ein passender branch gewählt werden.
Für die Entwicklung ist es sinnvoll, den Lübecker upstram lokal nach dem clone hinzufügen:
`git remote add upstream https://git.metameute.de/lff/firmware/`


## Build
`scripts/feeds update -a`

`scripts/feeds install -a`

`make` 


## Hinweis
Im Gegensatz zu lff bezieht sich dieses Repository auf die Upstream-Struktur, so wie sie Stand 2012-12-18 in Lübeck vorliegt. (lff bezieht sich auf den Stand vor Neoraiders refactoring).

