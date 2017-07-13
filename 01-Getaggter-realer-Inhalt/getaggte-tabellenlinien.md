---
tags: Microsoft Word, maschinelle Prüfung
---

## Problembeschreibung

Wird eine Tabelle aus Word 2013 exportiert, werden die Linien einer Tabelle innerhalb von `<Span>` Tags gesetzt. Ein `<Span>` Tag darf aber nicht innerhalb eines `<TR>` \(Tabellenzeile\) auf gleicher Ebene wie die `<TD>` Tags \(Tabellenzelle\) liegen. Zudem müssen Tabellenlinien als Artefakt ausgezeichnet sein und dürfen nicht getaggt werden.

Problem festgestellt bei der PDF-Konvertierung aus:

* Microsoft Word 2013 für Windows

### PAC 2 Fehlermeldung

> Invalid use of a Span structure element

### Prüfpunkt/e Matterhorn Protokoll

> **01-001** Artefakte sind als realer Inhalt getaggt.  
> **→ interaktive/semantische Prüfung**
>
> **09-004** Ein Strukturelement, das im Zusammenhang mit einer Tabelle steht, wird in einer Weise verwendet, die nicht mit Tabelle 337 der ISO 32000-1 übereinstimmt.  
> **→ automatische/technische Prüfung**

---

## Manueller Lösungsweg in Acrobat ![](/assets/icon_acrobat.gif)

1. Das Pfad Element wird als Artefakt gekennzeichnet. Dazu kann das Pfadelement, mithilfe eines Rechtsklicks in der Tag-Menüleiste, in ein aussertextliches Element geändert werden. 
2. Danach kann das leere `<Span>`Tag gelöscht werden.



