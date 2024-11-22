Erste Hilfe

# Erste Hilfe
  
Eine kurze Übersicht relevanter Themen für Problemlösungen und Supportfälle.

## Word-Vorlage erstellen
- Erstellen Sie eine neue Hauptvorlage.
- Fügen Sie in die Word-Vorlage Ihre Texte und Platzahlter hinzu.
  
### Platzhalter Hauptvorlage
In der Hauptvorlage können Sie die `Systemplatzhalter` als auch die `cobra Seriendruckfelder` für die Tabellen `Adresse` und `Rechnung` hinzufügen.
Die Platzhalter für die cobra Seriendruckfelder werden wie folgt aufgebaut: Sie setzen sich aus einem `Präfix`, dem cobra-Tabellennamen, und einem `Suffix`, dem Feldname, zusammen.
 
Die Tabellennamen finden Sie in den Einstellungen im gewünschten Format. Der Präfix für Adresse ist `Adressen`.
  
<img src="/docs/PräfixRechnung.webp" alt="Präfix Rechnung"/> 

Fügen Sie nun den Tabellennamen zusammen mit dem Feldnamen in Ihre Hauptvorlage ein. 

> [!NOTE]
> Die Systemplatzahlter finden Sie [hier](/Erste-Schritte/Vorlage+Platzhalter.md#platzhalter)

Zum Beispiel: `{E-Rechnung.Bestellnummer}`, `{E-Rechnung.Bemerkung}`, `{Adressen.Firma}`, `{Adressen.Adresskopf}` usw.

### Platzhalter Untervorlage
In der Untervorlage können Sie die `Systemplatzhalter` als auch die `cobra Seriendruckfelder` für die Tabellen `Position` und `ZU- und Abschlag` hinzufügen.
Die Platzhalter für die cobra Seriendruckfelder werden wie folgt aufgebaut: Sie setzen sich aus einem `Präfix`, dem cobra-Tabellennamen, und einem `Suffix`, dem Feldname, zusammen.

Die Tabellennamen finden Sie in den Einstellungen im gewünschten Format. 

<img src="/docs/PräfixPosition.webp" alt="Präfix Position"/> 

<img src="/docs/PräfixAbschlag.webp" alt="Präfix Abschlag"/>

> [!IMPORTANT]
> Die Platzhalter in der Untervorlage müssen innerhalb einer Tabelle eingefügt werden.

Fügen Sie nun den Tabellennamen zusammen mit dem Feldnamen in Ihre Untervorlage ein.

> [!NOTE]
> Die Systemplatzahlter finden Sie [hier](/Erste-Schritte/Vorlage+Platzhalter.md#platzhalter)

Zum Beispiel: `{E-Position.Bezeichnung}`, `{E-Rechnung.Menge}`, `{Zu- und Abschlag.Grund}`, `{Zu- und Abschlag.Betrag}` usw.

## XRechnung aus ZUGFeRD extrahieren mit Adobe Acrobat
 
- Öffnen Sie das ZUGFeRD-Dokument in Adobe Acrobat.
- Klicken Sie auf das :paperclip: (Büroklammer-Symbol), um die Anhänge im PDF anzuzeigen.
- Speichern Sie die Anlage `ZUGFeRD-invoice.xml` lokal auf Ihrem Rechner ab. 

<img src="/docs/Extrahieren.webp" alt="XRechnung extrahieren"/> 

## Problemlösungen

### Problem mit der Auflösung 

Treten bei Ihnen Probleme mit der Auflösung von cobra bzw. des Moduls auf, kann die Systemskalierung - falls die Skalierung mehr als 100% beträgt - der Auflösung Ihres Computers eine Ursache sein.

<img src="https://faktura-modul-ch.cobra-hilfe.de/images/faktura/loesung.webp" alt="System Bildschirm"/> 

- Rufen Sie die Eigenschaften der Datei `cobra.exe` auf.
- Wechseln Sie in den Reiter `Kompatibilität`.
- Klicken Sie auf die Schaltfläche `Hohe DPI-Einstellungen ändern`.
- Aktivieren Sie die Option `Außerkraftsetzung der hoher DPI-Skalierung`.
- Wählen Sie unter `Skalierung durgeführt von` die Möglichkeit `System` aus.
- Übernehmen Sie Ihre Änderungen und schließen Sie die Dialoge.

<img src="https://faktura-modul-ch.cobra-hilfe.de/images/faktura/loesung1.webp" alt="Hohe DPI-Einstellungen"/> 
 

## 
 
[Nächste](./)
 
