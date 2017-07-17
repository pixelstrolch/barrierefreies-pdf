---
Tags: Adobe InDesign, Microsoft Word, technische Prüfung
---

## Problembeschreibung

In sogenannten «schwach strukturierten Dokumenten» werden nummerierte Überschriften-Tags eingesetzt. Die Tags sehen so aus: `<Hn>`, wobei `n` für eine Ziffer von 1 bis 6 steht. Mithilfe der nummerierten Überschriften-Tags wird eine Struktur und Hierarchie im Dokument hergestellt.

Damit alle die Struktur nachvollziehen können, dürfen Überschriftenebenen nicht übersprungen werden. Nach einer `<H1>` darf demnach nicht direkt eine `<H3>` folgen. Jedoch kann nach einer `<H3>` wieder eine `<H1>` folgen da beispielsweise ein neues Kapitel beginnt.

### PAC 2 Fehlermeldung

> Numbered heading skips one ore more heading levels

### Prüfpunkt/e Matterhorn Protokoll

> **14-003** Bei nummerierten Überschriften-Tags in absteigender Folge wird eine Ebene übersprungen  
> **→ technische Prüfung**

---

## Manueller Lösungsweg in Word

Die Überschriftenebenen können mithilfe der Formatvorlagen bestimmt werden, siehe [«Mithilfe von Word-Formatvorlagen die PDF-Tags bestimmen»](#). Beim Auftreten dieses Fehlers müssen die angewendeten Formatvorlagen korrigiert werden und eventuell der bestehende Formatvorlagenkatalog überdenkt werden.

Ein hilfreiches Werkzeug ist der Navigationsbereich. Falls dieser nicht sichtbar ist, kann dieser im Menü _«Ansicht»_ aktiviert werden.

## Manueller Lösungsweg in InDesign

Die Überschriftenebenen können mithilfe der Formatvorlagen bestimmt werden, siehe [«Mithilfe der InDesign-Absatzformate die PDF-Tags bestimmen»](/mithilfe-der-indesign-absatzformate-die-pdf-tags-bestimmen.md). Beim Auftreten dieses Fehlers müssen die angewendeten Formatvorlagen korrigiert werden und eventuell der bestehende Formatvorlagenkatalog überdenkt werden.

## Manueller Lösungweg in Acrobat

Der vermutlich aufwendigste und unübersichtlichste Lösungsweg ist die Korrekturen im Tagbaum von Acrobat vorzunehmen. 

