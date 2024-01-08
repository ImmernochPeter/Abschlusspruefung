# Modelle und Diagramme (LF8)

Inhalte zum Kapitel Modelle und Diagramme

Inhalte basierend auf dem Unterricht von Herrn Burggraf

[zurück](/LF08/lf8.md)

## Inhalte

- [Modelle und Diagramme (LF8)](#modelle-und-diagramme-lf8)
  - [Inhalte](#inhalte)
  - [Entity-Relationship-Modell - ERM](#entity-relationship-modell---erm)
    - [Grundelemente](#grundelemente)
  - [Relationales Datenbankmodell](#relationales-datenbankmodell)

## Entity-Relationship-Modell - ERM

+ Grundlage für Datenbankentwurf
+ Planung, wie Datenbankstruktur aufgebaut und funktionieren soll
+ gängiger Standard für Datenmodellierung
+ Typisierung von Objekten, ihrer relationalen Beziehung untereinander und überführenden Attribute

### Grundelemente

![alt ERM Bild 1](/LF08/images/erm.png)
*Abb. Entity-Relationship-Modell* <br>
<sub>Datenbanken verstehen für Anfänger und Profis. </sub>

+ Entität = individuell identifizierbares Objekt der Wirklichkeit
+ Beziehung = Verknüpfung / Zusammenhang zwischen zwei / mehreren Entitäten
+ Attribut = Eigenschaft, die im Kontext zu Entität steht
+ Kardinalität = beschreibt Beziehung zwischen Attributen (1:1, 1:n, m:n)

**1:1**
+ jeder Datensatz in Tabelle A wird genau einem Datensatz in Tabelle B zugeordnet und umgekehrt
+ sollte in Modellierung vermieden werden, da solche Informationen meistens auch in einer Tabelle sein können
+ wird nur verwendet, um Tabelle aufgrund von Komplexität zu teilen, oder um Teil der Tabelle aus Gründen der Zugriffsrechte zu isolieren

**1:n**
+ häufigster Beziehungstyp in Datenbanken
+ einem Datensatz aus Tabelle A können mehrere passende Datensätze in Tabelle B zugeordnet sein
+ einem Datensatz in Tabelle B kann nur einem Datensatz in A zugeordnet sein

**m:n**
+ jedem Datensatz in Tabelle A mehrere passende Datensätze in Tabelle B zugeordnet und umgekehrt
+ können nur über eine dritte Tabelle *Verbindungstabelle C* realisiert werden
+ Verbindungstabelle enthält in der Regel nur Fremdschlüssel der anderen Tabellen
+ Primärschlüssel der Verbindungstabelle wird aus diesen beiden Fremdschlüsseln gebildet

![alt ERM-Beispiel Bild 1](/LF08/images/erm-example.png)
*Abb. Beispiel eines Entity-Relationship-Modells* <br>
<sub>Gratzke, J. (Hg.): IT-Berufe. Grundstufe 1. Jahr. Westermann Verlag Braunschweig 2020. </sub>

## Relationales Datenbankmodell

