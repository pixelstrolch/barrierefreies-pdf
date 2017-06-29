# Problembeschreibung ![](/assets/icon_word.gif)

Ein Inhaltsverzeichnis wird mit den Tags `<TOC>` und `<TOCI>` erstellt. `<TOC>` ist dabei der Container und `<TOCI>` wird für die einzelnen Einträge verwendet. Bei diesem Fehlerszenario werden im PDF einzelne Einträge innerhalb Überschriften-Tags, z.B. `<H1>`, anstatt `<TOCI>` strukturiert.

Problem festgestellt bei der PDF-Konvertierung aus:

* Microsoft Word 2013 für Windows

## PAC 2 Fehlermeldung

Keine Warnung oder Fehlermeldung zu diesem Problem!

## Prüfpunkt/e Matterhorn Protokoll

> **01-006** Der Strukturtyp und Attribute eines Strukturelementes sind nicht semantisch geeignet für das Strukturelement. Alle Strukturelemente müssen in Betracht gezogen werden.  
> **→ interaktive/semantische Prüfung**

---

# Manueller Lösungsweg in Word ![](/assets/icon_word.gif)

Word verwendet für die einzelnen Verzeichniseinträge die Formatvorlagen _Verzeichnis 1_, _Verzeichnis 2_, usw. Ist in diesen Formatvorlagen die Gliederungsebene \(Absatz Einstellungen\) nicht als Textkörper definiert, werden die Überschriften-Tags angewendet. Diese müssen also zwingend mit der Option Textkörper definiert sein.

