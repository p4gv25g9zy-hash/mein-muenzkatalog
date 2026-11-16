# Mein Münzkatalog – iPhone-Web-App

## Funktionen
- Einträge für Münzen und Medaillen mit Land, Jahrgang, Menge, Gewicht, Silberanteil und Kaufpreis
- Fotos von Vorder- und Rückseite direkt mit iPhone-Kamera/Fotomediathek
- automatische Summen: Stück, Bruttogewicht, Feinsilber, Anschaffungskosten und rechnerischer Materialwert
- Silberkurs-Aktualisierung über XAG in USD/Feinunze plus USD/EUR-Umrechnung
- Excel-kompatibler CSV-Export, PDF über iOS-Druckdialog
- JSON-Backup mit Fotos und Wiederherstellung
- Offline-App-Shell nach erstem Laden; lokale Datenbank (IndexedDB)

## Auf dem iPhone installieren
Eine PWA muss über eine HTTPS-Adresse bereitgestellt werden. ZIP-Datei entpacken und alle Dateien in einen statischen Webhost laden (z. B. GitHub Pages oder einen anderen HTTPS-Webhost). Danach auf dem iPhone:
1. Die HTTPS-Adresse in Safari öffnen.
2. Teilen antippen.
3. „Zum Home-Bildschirm“ wählen.
4. „Als Web-App öffnen“ aktivieren, falls angeboten, und „Hinzufügen“ tippen.

## Wichtige Hinweise
- Die Web-App kann nicht direkt aus einer ZIP-Datei als installierte Home-Bildschirm-App gestartet werden.
- Einträge und Fotos liegen lokal im Safari-/Web-App-Speicher dieses iPhones. Browserdaten löschen oder die Web-App entfernen kann Daten gefährden. Regelmäßig JSON-Backups exportieren.
- Keine Cloud-Synchronisierung.
- Der automatische Silberkurs nutzt `api.gold-api.com` (XAG) und `api.frankfurter.app` (USD/EUR). Verfügbarkeit, CORS-Freigabe und Aktualität der Drittanbieter sind nicht garantiert. Der Preis kann jederzeit manuell angepasst werden.
- PDF: Die Druckfunktion öffnet den iOS-Druckdialog. Im Druckdialog die Vorschau mit zwei Fingern vergrößern und dann über Teilen als PDF sichern.
- CSV ist eine Excel-kompatible Texttabelle, keine native XLSX-Datei.
- Das Projekt ist nicht signiert und nicht im App Store veröffentlicht.
