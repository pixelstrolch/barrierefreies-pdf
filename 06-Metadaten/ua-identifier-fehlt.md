---
tags: Adobe InDesign, Microsoft Word, technische Prüfung
---

## Problembeschreibung

Damit ein PDF-Dokument als technisch barrierefrei gilt, muss die Metainformation vorhanden sein, welche das Dokument als PDF/UA kompatibel kennzeichnet.

Problem festgestellt bei der PDF-Konvertierung aus:

* Microsoft Word 2013 für Windows
* Adobe InDesign alle Versionen

### PAC 2 Fehlermeldung

> PDF/UA identifier missing

### Prüfpunkt/e Matterhorn Protokoll

> **06-002** Der Metadata-Datenstrom im Catalog-Dictionary enthält keine PDF/UA-Kennzeichnung.  
> **→ technische Prüfung**

---

## Manueller Lösungsweg in Acrobat

1. Die Datei [pdfUA-ID.xmp herunterladen](https://taggedpdf.com/xmp/pdfUA-ID.xmp)
2. Das betroffene Dokument in Acrobat öffnen
3. Die Dokumenteigenschaften anzeigen \(Datei → Eigenschaften\)
4. In das Register _«Beschreibung»_ wechseln und den Button _«Zusätzliche Metadaten»_ klicken
5. In das Register _«Erweitert»_ wechseln und den Button _«Anhängen»_ klicken
6. Die vorgängig heruntergeladene Datei _«pdfUA-ID.xmp»_ auswählen und «Öffnen» klicken

## Automatischer Lösungsweg in Acrobat DC

1. Das Werkzeug-Register _«Druckproduktion»_ öffnen und auf _«Preflight»_ klicken
2. Im Preflight-Fenster die Preflight Korrekturen anzeigen \(auf den kleinen Button mit dem Schraubenschlüssel Symbol klicken\)
3. Die Korrektur _«PDF/UA-1-Eintrag setzen»_ auswählen und auf den Button _«Korrigieren»_ klicken

Diese Korrektur ist ausserdem Bestandteil des Preflight-Profils _«Strukturprobleme getaggter PDF-Dokumente beheben»_.

## Automatischer Lösungsweg in InDesign \(MadeToTag\)

Mit der Verwendung des Plugins MadeToTag wird die Metadaten-Information automatisch angehängt.

