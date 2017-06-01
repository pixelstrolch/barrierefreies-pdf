## Problembeschreibung ![](/assets/icon_word.gif)

Ein Bild wird in Word **im Kompatibilitätsmodus** \(.doc\) eingefügt und mit der Layoutoption _**«Mit Text in Zeile»**_ platziert. Nach dem PDF-Export ist das Bild nicht wie erwartet innerhalb eines `<Figure>` Tags, sondern innerhalb eines `<InlineShape>`, welchem die  Rolle `<Sect>` zugeordnet ist.

Problem festgestellt bei der PDF-Konvertierung aus:

* Microsoft Word 2013 für Windows \(im Kompatibilitätsmodus\)

### PAC 2 Warnung

> Possibly inappropriate use of a Sect structure element

### **Prüfpunkt/e Matterhorn Protokoll**

> **13-001** Grafikobjekte, bei denen es sich weder um Textobjekte noch um Artefakte handelt, sind nicht als Figure getaggt.  
> **→ interaktive/semantische Prüfung**

---

## Manueller Lösungsweg in Acrobat ![](/assets/icon_acrobat.jpg)

1. Mit dem TouchUp-Leserichtung-Werkzeug kann das Bild ausgewählt und in eine Abbildung umgewandelt werden. 
2. Der nicht standardisierte Tag `<InlineShape>` wird so zu einem `<Figure>` umgewandelt. 
3. Der Alternativtext wird automatisch übernommen.

## Automatischer Lösungsweg in Word 2013 ![](/assets/icon_word.gif)

Da das Problem nur im _.doc-Format_, respektive im Kompatibilitätsmodus besteht, kann das Dokument in das neuere _.docx-Format_ konvertiert werden. Der Befehl _«Konvertieren»_ befindet sich im Menü _«Datei»_ im Register _«Informationen»_.

Achtung: Die Konvertierung kann \(geringere\) Layoutveränderungen verursachen!

