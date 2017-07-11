# Problembeschreibung ![](/assets/icon_word.gif) ![](/assets/icon_indesign.gif)

In sogenannten «schwach strukturierten Dokumenten» werden nummerierte Überschriften-Tags eingesetzt. Die Tags sehen so aus: `<Hn>`, wobei `n` für eine Ziffer von 1 bis 6 steht. Mithilfe der nummerierten Überschriften-Tags wird eine Struktur und Hierarchie im Dokument hergestellt.

Damit alle die Struktur nachvollziehen können, dürfen Überschriftenebenen nicht übersprungen werden. Nach einer `<H1>` darf demnach nicht direkt eine `<H3>` folgen. Jedoch kann nach einer `<H3>` wieder eine `<H1>` folgen da beispielsweise ein neues Kapitel beginnt.

## PAC 2 Fehlermeldung

> Numbered heading skips one ore more heading levels

## Prüfpunkt/e Matterhorn Protokoll

> **14-003** Bei nummerierten Überschriften-Tags in absteigender Folge wird eine Ebene übersprungen  
> **→ automatische/technische Prüfung**

---

# Manueller Lösungsweg in Word ![](/assets/icon_word.gif)

In den Absatzeinstellung wird die Gliederungsebene definiert. Dort kann die Ebene 1–6 ausgewählt werden und steuert damit beim PDF-Export die Überschriftenebene.

Am einfachsten verwendet man die Standardformatvorlagen _«Überschrift 1»_ bis _«Überschrift 6»_, welche bereits die korrekte Ebene hinterlegt haben.

Die Ebenenstruktur kann mithilfe des Navigationsbereich nachvollzogen werden. Falls dieser nicht sichtbar ist, fehlt das Häckchen unter dem Menü _«Ansicht»_.

# Manueller Lösungsweg in InDesign ![](/assets/icon_indesign.gif)

In InDesign kann die Überschriftsebene innerhalb der Einstellungen einer Absatzformatvorlage definiert werden. Unter _«Tagsexport»_ können die Tags für den PDF- sowie auch dem HTML/EPUB-Export definiert werden.

Im Menü des Panels _«Absatzformate»_ befindet sich der Befehl _«Alle Exporttags bearbeiten»_. Damit können, innerhalb einer Liste aller Absatzformate, alle Exporttags auf einmal vergeben werden.

