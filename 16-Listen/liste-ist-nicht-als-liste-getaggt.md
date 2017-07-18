---
tags: 'Adobe Indesign, Microsoft Word, semantische Prüfung'
---

## Problembeschreibung

Wenn undefinierte oder nummerierte Listen verwendet werden, sollen diese auch als Liste getaggt werden. Die Listen-Tags werden beim Export aus Microsoft Word oder Adobe InDesign automatisch vergeben, sofern die Listen korrekt erstellt wurden.

Für eingeschränkte Menschen sind korrekt getaggte Listen wertvoll und verbessern die Navigationsmöglichkeiten.

### PAC 2 Fehlermeldung

Keine Warnung oder Fehlermeldung zu diesem Problem!

### **Prüfpunkt/e Matterhorn Protokoll**

> **01-006** Der Strukturtyp und Attribute eines Strukturelementes sind nicht semantisch geeignet für das Strukturelement. Alle Strukturelemente müssen in Betracht gezogen werden. → semantische Prüfung  
> **16-003** Inhalt ist eine Liste, die jedoch nicht als Liste getaggt  
> ist. → semantische Prüfung

---

## Manueller Lösungsweg in Word

Die betroffenen Stellen können mit der Listenfunktion umformatiert werden.

![Listen-Schaltflächen in Microsoft Word](/assets/listen_word.png)

Um eine einheitliche Formatierung zu gewährleisten, wird das Anlegen einer Listenformatvorlage empfohlen.

## Manueller Lösungsweg in InDesign

Die betroffenen Stellen können mit der Listenfunktion umformatiert werden.

![Listen-Schaltflächen in Adobe InDesign](/assets/listen_indesign.png)

Um eine einheitliche Formatierung zu gewährleisten, wird die Verwendung einer separaten Absatzformatvorlage empfohlen.

## Manueller Lösungsweg in Acrobat

Das manuelle Nachtaggen von Listen ist zeitaufwändig. Es wird empfohlen eine der oben stehenden Lösungswege vorzuziehen. Die benötigten Tags sind `<L>`, `<LI>`, `<Lbl>` und `<LBody>`.

