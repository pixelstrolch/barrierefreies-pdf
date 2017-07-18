---
tags: 'Microsoft Word, technische Prüfung'
---

## Problembeschreibung

Bilder in Word-Dokumenten werden beim PDF-Export immer auf Block-Ebene ausgegeben. Dem `<Figure>` Tag werden keine zusätzliche Attribute mitgegeben, welche es als Block-Element kennzeichnen. PAC 2 gibt in diesen Fall unten stehende Warnung aus.

Problem festgestellt bei der PDF-Konvertierung aus:

* Microsoft Word 2013 für Windows
* Microsoft Word für Mac \(mind. bis Version 15.33\)

### PAC 2 Warnung

> _Possibly inappropriate use of a Figure structure element_

### Prüfpunkt/e Matterhorn Protokoll

Ist nicht Bestandteil des Matterhorn Protokolls.

---

## Manueller Lösungsweg in Acrobat

Schnellster und einfachster Weg ist es das `<Figure>` Tag nicht als eigenständiges Block-Element zu behandeln.

Dazu kann das `<Figure>` Tag

* innerhalb des zugehörigen Absatz \(`<P>` Tag\) verschoben werden oder 
* ein neues `<P>` Tag erstellt werden und das `<Figure>` Tag darin verschoben werden.

Zu beachten gilt, dass die Lesereihenfolge \(Reihenfolge der Tags\) danach immer noch korrekt sein muss.

## Manueller Lösungsweg 2 in Acrobat

1. In den Eigenschaften des `<Figure>` Tags auf «_Attributobjekte bearbeiten…_» klicken
2. Auf das Pluszeichen links von «_Attributobjekte_» klicken
3. Die nächst untere Ebene \(Attributobjekt 1\) markieren und den Button _«Neues Element»_ klicken
4. Das Dialogfeld wie folgt ausfüllen:
   * Schlüssel: Placement
   * Wert: Block
   * Werttyp: Name

