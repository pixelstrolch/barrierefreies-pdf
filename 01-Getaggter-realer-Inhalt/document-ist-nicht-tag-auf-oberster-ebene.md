---
tags: Microsoft Word
---

## Problembeschreibung

Ein aus Word 2013 konvertiertes PDF enthält als oberstes Container das `<Part>` Tag. Die oberste Ebene sollte jedoch mit einem `<Document>` Tag strukturiert werden.

Problem wurde festgestellt bei der PDF-Konvertierung aus:

* Microsoft Word 2013 für Windows

### PAC 2 Warnung

> Part structure element used as root element

### Prüfpunkt/e Matterhorn Protokoll

> **01-006** Der Strukturtyp und Attribute eines Strukturelementes sind nicht semantisch geeignet für das Strukturelement. Alle Strukturelemente müssen in Betracht gezogen werden.  
> **→ interaktive/semantische Prüfung**

---

## Manueller Lösungsweg 1 in Acrobat ![](/assets/icon_acrobat.gif)

1. Das betroffene Tag im Tagbaum einmal anklicken um es auszuwählen.
2. Mit der Maus erneut auf das ausgewählte Tag klicken um es umzubenennen.
3. Den Tag `<Part>` in `<Document>` umbenennen.

![Animation zeigt die drei Schritte des manuellen Lösungswegs 1 in Acrobat](/assets/pdf-tag-umbenennen.gif)

## Manueller Lösungsweg 2 in Acrobat ![](/assets/icon_acrobat.gif)

1. Rechtsklick mit der Maus auf das betroffene Tag im Tagbaum.
2. Im Menü die Eigenschaften auswählen.
3. Im Eigenschaften-Fenster, im Register Tag, kann der Typ auf _«Dokument»_ \(übersetzte Schreibweisung\) geändert werden.

![Animation zeigt die drei Schritte des manuellen Lösungswegs 2 in Acrobat](/assets/pdf-tag-umbennnen-2.gif)

