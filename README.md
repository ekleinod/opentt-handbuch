# OpenTT-Handbuch

Handbuch für Spielverantwortliche (eine deutsche Übersetzung des "Handbook for Match Officials")

Teil des Projekts "OpenTT", offene Dokumente und Programme rund um Tischtennis.

Lizenz: Creative-Commons-Lizenz Namensnennung - Nicht-kommerziell - Weitergabe unter gleichen Bedingungen 4.0 International

Siehe Datei LICENSE.

## Was soll das? Kann ich mitmachen?

Ich will das "Handbook for Match Officials" auf Deutsch in einem schönen Dokument zur Verfügung stellen, das auch in verschiedene Formate umgewandelt werden kann, z.B. als PDF-Datei oder HTML.
Dafür werden die Regeln in *Multimarkdown* geschrieben und dann umgewandelt.

*Multimarkdown* habe ich gewählt, da so jeder einfach Änderungen schreiben und mir zukommen lassen kann.
Wer mit Git umgehen kann, dann dies sogar direkt tun.

## Technische Details

### Benötigte Programme

Editieren

- Editor Ihrer Wahl, muss UTF-8 können

Multimarkdown

- Multimarkdown-Programm von http://fletcherpenney.net/multimarkdown/

LaTeX

- LaTeX-Distribution (z.B. MiKTeX http://www.miktex.org/ oder TeXLive http://www.tug.org/texlive/)
- Basis-Stil von https://github.com/ekleinod/basis

Ant

- zur Automatisierung der Dokumenterzeugung von http://ant.apache.org/

### Git-Repository

Kurze Details zum Aufbau des Git-Repositories:
Die Aufteilung in Zweige orientiert sich am Git-Branching-Modell, das in http://nvie.com/posts/a-successful-git-branching-model/ beschrieben wird.

Das heißt, es gibt immer mindestens drei Zweige:

1. `master` - enthält nur fertige Versionen
2. `develop` - Hauptzweig, gegen den entwickelt wird, dient der Synchronisation der feature-, release- und hotfix-Zweige
3. `feature-work` - Haupt-Arbeitszweig, in dem standardmäßig geschrieben wird

Zusätzlich werden bei Bedarf folgende Zweige genutzt:

- `feature-*` - für das Schreiben eines bestimmten Features/Textteils
- `release-*` - Synchronisation fertiger Versionen zwischen `develop` und `master`
- `hotfix-*` - schnelle Fehlerbehebung


