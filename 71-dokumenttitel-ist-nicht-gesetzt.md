## Problembeschreibung ![](/assets/icon_word.jpg) ![](/assets/icon_indesign.jpg)

In den PDF-Dokumenteigenschaften kann definiert werden ob das Dokument mit dem Dateinamen oder dem Dokumenttitel angezeigt wird. Dieser erscheint im PDF-Viewer als Name des Dokumentfensters oder wird mit einem Screenreader als erste Information vorgelesen. PDFs, welche aus Microsoft Word und Adobe InDesign hergestellt werden, zeigen den Dateinamen. Nach PDF/UA ist jedoch der Dokumenttitel einzustellen da dieser aussagekräftiger ist.

Problem festgestellt bei der PDF-Konvertierung aus:

* Microsoft Word 2013 für Windows
* Adobe InDesign bis CC 2015 \(ab Version CC 2015 steht eine Option im Exportfenster zur Verfügung\)

### PAC 2 Fehlermeldung

> DisplayDocTitle key is not set to true

### **Prüfpunkt/e Matterhorn Protokoll**

> **07-001** Das ViewerPreferences-Dictionary des Catalog-Dictionary enthält keinen Schlüssel DisplayDocTitle.  
> **07-002** Das ViewerPreferences-Dictionary des Catalog-Dictionary enthält einen Schlüssel DisplayDocTitle mit dem Wert false.  
> **→ automatische/technische Prüfung**

---

## Manueller Lösungsweg in Acrobat ![](/assets/icon_acrobat.jpg)

1. Das betroffene Dokument in Acrobat öffnen

2. Die Dokumenteigenschaften anzeigen \(Datei → Eigenschaften\)

3. In das Register _Ansicht beim Öffnen_ wechseln und unter _Einblenden_ den Wert auf _Dokumenttitel_ wechseln

## Automatischer Lösungsweg in InDesign \(ab CC 2015\) ![](/assets/icon_indesign.jpg)

Seit Adobe InDesign CC 2015 wird in den PDF-Export-Einstellungen ein neuer Bereich mit dem Namen _Barrierefreiheitsoptionen_ im Register _Erweitert_ angezeigt. Darin kann der anzuzeigende Namen in _Dokumenttitel_ geändert werden.

## Automatischer Lösungsweg in InDesign \(mit Plugin MadeToTag\) ![](/assets/icon_indesign.jpg)

Mit der Verwendung des Plugins MadeToTag wird der Dokumenttitel automatisch definiert.

