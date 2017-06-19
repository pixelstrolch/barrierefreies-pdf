## Problembeschreibung ![](/assets/icon_word.gif)

In PDFs, welche aus Word 2013 exportiert werden, fehlt bei allen vorhandenen Bildern die Bounding Box Attribute.

Problem festgestellt bei der PDF-Konvertierung aus:

* Microsoft Word 2013 für Windows

### PAC 2 Fehlermeldung

> Figure element on a single page with no bounding box

### **Prüfpunkt/e Matterhorn Protokoll**

Ist nicht Bestandteil des Matterhorn Protokolls.

---

## Manueller Lösungsweg in Acrobat ![](/assets/icon_acrobat.gif)

1. Alternativtext des betroffenen Bildes kopieren \(Tag-Baum → Rechtsklick auf betroffenes `<Figure>` → Eigenschaften → Tag\)
2. `<Figure>` Tag löschen
3. `<Figure>` Tag neu mit Touch-Up Werkzeug neu anlegen
4. Alternativtext in neuem `<Figure>` einfügen \(Tag-Baum → Rechtsklick auf betroffenes `<Figure>` → Eigenschaften → Tag\)
5. Ist das `<Figure>` Tag nicht innerhalb eines Block-Elements, wie z.B. `<P>`, gegliedert, so wird die Warnung «_Possibly inappropriate use of a Figure structure element_» ausgegeben. Wenn das Bild als alleinstehendes Block-Element verwendet werden soll, so kann folgendes getan werden:
   1. In den Eigenschaften des `<Figure>` Tags auf _«Attributobjekte bearbeiten…»_ klicken
   2. Auf das Pluszeichen links von «_Attributobjekte_» klicken
   3. Die nächst untere Ebene \(Attributobjekt 1\) markieren und den Button _«Neues Element»_ klicken
   4. Das Dialogfeld wie folgt ausfüllen:
      * Schlüssel: Placement
      * Wert: Block
      * Werttyp: Name



