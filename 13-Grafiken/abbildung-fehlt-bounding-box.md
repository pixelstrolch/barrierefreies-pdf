# Problembeschreibung ![](/assets/icon_word.gif)

In PDFs, welche aus Word exportiert werden, fehlen bei allen vorhandenen Bildern die Bounding Box Attribute, egal mit welcher Layoutoption sie platziert wurden.

Problem festgestellt bei der PDF-Konvertierung aus:

* Microsoft Word 2013 für Windows
* Microsoft Word für Mac \(mind. bis Version 15.33\)

## PAC 2 Fehlermeldung

> Figure element on a single page with no bounding box

## Prüfpunkt/e Matterhorn Protokoll

Ist nicht Bestandteil des Matterhorn Protokolls.

---

# Manueller Lösungsweg in Acrobat ![](/assets/icon_acrobat.gif)

1. Alternativtext des betroffenen Bildes kopieren \(Tag-Baum → Rechtsklick auf betroffenes `<Figure>` → Eigenschaften → Tag\)
2. `<Figure>` Tag löschen
3. `<Figure>` Tag neu mit Touch-Up Werkzeug neu anlegen
4. Alternativtext in neuem `<Figure>` einfügen \(Tag-Baum → Rechtsklick auf betroffenes `<Figure>` → Eigenschaften → Tag\)

Für die Warnung «_Possibly inappropriate use of a Figure structure element_», siehe [_«13.4 Figure als Block-Element»_](/134-abbildung-als-block-element.md).

