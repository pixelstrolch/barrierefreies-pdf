## Problembeschreibung

Wenn PAC2 die Warnung _«Part structure element used as root element»_ ausgibt, wurde mit höchster Wahrscheinlichkeit ein Word-Dokument exportiert. In Word 2013 werden sämtliche Inhalte innerhalb eines `<Part>` Container-Tag strukturiert. Die oberste Ebene sollte jedoch mit einem `<Document>` Tag erstellt werden.

### Bet**roffene/r Prüfpunkt/e des Matterhorn Protokolls**

> 01-006: Der Strukturtyp und Attribute eines Strukturelementes sind nicht semantisch geeignet für das Strukturelement. Alle Strukturelemente müssen in Betracht gezogen werden.  
> **→ Interaktive, semantische Prüfung**

### Betroffene Software

* Microsoft Word

### Manueller Lösungsweg in Acrobat

* Das betroffene Tag im Tagbaum mittels Doppelklick überschreiben oder
* Das betroffene Tag im Tagbaum auswählen und mit Rechtsklick die Eigenschaften aufrufen. Im Eigenschaften-Fenster kann das Tag unter Typ geändert werden.

### 

### 

## 

## 



