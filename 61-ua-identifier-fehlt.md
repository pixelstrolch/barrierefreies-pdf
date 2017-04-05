## Problembeschreibung

![](/assets/icon_word.jpg)  ![](/assets/icon_indesign.jpg)

Damit ein PDF-Dokument als technisch barrierefrei gilt, müssen ihm zusätzliche Metainformationen hinzugefügt werden. Dies ist eine Kennzeichnung, dass das Dokument mit dem PDF/UA Standard kompatibel ist.

PAC 2 gibt bei diesem Problem die Fehlermeldung _**«PDF/UA identifier missing»**_ aus.

Problem festgestellt bei der PDF-Konvertierung aus:

* Microsoft Word alle Versionen
* Adobe InDesign alle Versionen

### **Prüfpunkt/e Matterhorn Protokoll**

> **06-002** Der Metadata-Datenstrom im Catalog-Dictionary enthält keine PDF/UA-Kennzeichnung.  
> **→ automatische/technische Prüfung**

## Manueller Lösungsweg in Acrobat

## ![](/assets/icon_acrobat.jpg)

1. Die Datei [pdfUA-ID.xmp herunterladen](https://taggedpdf.com/xmp/pdfUA-ID.xmp)

2. Das betroffene Dokument in Acrobat öffnen

3. Die Dokumenteigenschaften anzeigen \(Datei → Eigenschaften\)

4. In das Register «Beschreibung» wechseln und den Button «Zusätzliche Metadaten» klicken

5. In das Register «Erweitert» wechseln und den Button «Anhängen» klicken

6. Die vorgängig heruntergeladene Datei «pdfUA-ID.xmp» auswählen und «Öffnen» klicken

## Manueller Lösungsweg in Acrobat DC

## ![](/assets/icon_acrobat.jpg)

1. Das Werkzeug-Register «Druckproduktion» öffnen und auf «Preflight» klicken

2. Im Preflight-Fenster auf den kleinen Button mit dem Schraubenschlüssel Symbol klicken

3. In die Gruppe «Dokumentinformationen und Metadaten» navigieren

4. Das Profil «PDF/UA-1-Eintrag setzen» auswählen und auf den Button «Korrigieren» klicken

## Automatischer Lösungsweg in InDesign

![](/assets/icon_indesign.jpg)

Mit der Verwendung des Plugins MadeToTag werden die Metadaten automatische angehängt.

