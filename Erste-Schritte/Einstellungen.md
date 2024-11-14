Erste Schritte

# Einstellungen 

## automatische Generierung

> [!TIP]
> Für Testzwecke empfehlen wir, zunächst die automatische Generierung der Datenbankstruktur zu nutzen, bevor Sie mit der individuellen Konfiguration beginnen. Diese Option wird Ihnen beim ersten Klick auf `Einstellungen` angeboten.
>  
> <img src="/docs/Datenbankstruktur.png" alt="Datenbankstruktur" height="150"/> 
> 
> - Zusätzlich zur Datenbankstruktur werden Demodaten, ein Demo-Format, eine Demoansicht und ein Demo-Serien-E-Mail-Format angelegt. So können Sie direkt mit dem Testen beginnen.
> 
> - Ab CRM PRO kann die automatisch generierte Positionstabelle über ein Beziehungsfeld mit einer Artikeltabelle (Freientabelle) verknüpft werden.
> 
>   <img src="/docs/Artikeltabelle.png" alt="Artikeltabelle.png" height="150"/> 
> 
> - Optional lässt sich eine einfache Kopierregel zusammenstellen.
>
>   <img src="/docs/Kopierregel.png" alt="Kopierregel" /> 
> 
>   - Wählen Sie die gewünschte Artikeltabelle aus.
>   - Ordnen Sie die gewünschten Felder der Artikeltabelle der Positionstabelle zu.
>   - Bestätigen Sie Ihre Eingabe mit `OK`.
> 
> - Nach der automatischen Generierung müssen Sie cobra neu starten.
> 
> - Zum Schluss konfigurieren Sie die Verkäuferdaten, Zahlungsdetails und das Dokumentenfeld in der Rechnungstabelle gemäß Ihren Schlagwörtern.
>   - Optional können Sie [Eingabemasken](https://eingabemasken.cobra-hilfe.de/), Ansichten, Kopierregeln und Anzeigeformat an Ihre Ansprüche anpassen.
 
## individuelle Konfiguration

In diesem Kapitel wird beschrieben, wie Sie eine individuelle Konfiguration vornehmen, um ein Format zu erstellen. Klicken Sie im Menüband auf `Einstellungen`, um die Konfiguration zu öffnen.

## Neues Format 

Um ein neues Format zu erstellen, klicken Sie bei `Format` auf das Pluszeichen (+).

<img src="/docs/Neu.png" alt="Neu"/> 

- Geben Sie dem Format einen Namen. 
- Wenn Sie die Einstellungen des aktuellen Formats übernehmen möchten, können Sie es duplizieren.
- Bestätigen Sie Ihre Eingabe mit `OK`.

## Format Löschen

Um ein Format zu löschen, klicken Sie bei `Format` auf das X-Symbol (X).

<img src="/docs/Löschen.png" alt="Löschen"/> 

- Bestätigen Sie Ihre Eingabe mit `Ja`.

## Rechnung

<img src="/docs/Allgemein.webp" alt="Rechnung"/> 

Feld | Beschreibung |
:-- | :--
Rechnung* | Wählen Sie hier Ihre Rechnungstabelle.
Rechnungsnummer* | Geben Sie hier die eindeutige Nummer der Rechnung ein.
Rechnungsdatum* | Wählen Sie hier das Datum aus, an dem die Rechnung ausgestellt wurde.
Abrechnungszeitrum | Wählen Sie `Abrechnungszeitraum`, wenn es sich um einen Zeitraum handelt. 
Von* | Wählen Sie hier das Startdatum des Abrechnungszeitraums aus.
Bis* | Wählen Sie hier das Enddatum des Abrechnungszeitraums aus.
Liefer-/Leistungsdatum* | Wählen Sie hier das Datum aus, an dem die Ware geliefert oder die Dienstleistung erbracht wird.
E-Mail für Versand | Die E-Mail des Käufers wird in dieses Feld kopiert, um es für den E-Mail-Versand zu verwenden.
Fälligkeitsdatum | Wählen Sie hier das Datum aus, an dem die Rechnung fällig wird. Das Datum darf nicht in der Vergangenheit liegen.
Projektkennung | Geben Sie hier die Nummer des Projekts ein, in dessen Rahmen die Rechnung gestellt wird.
Vertragsnummer | Geben Sie hier die Nummer des Vertrages ein, in dessen Rahmen die Rechnung gestellt wird.
Bestellnummer | Geben Sie hier die Nummer der Bestellung des Käufers ein, in deren Rahmen die Rechnung gestellt wird.
Bemerkung | Hier können Sie rechnungserklärende Bemerkungen einfügen.

## Dokument

<img src="/docs/Dokument.png" alt="Dokument"/> 

Feld | Beschreibung |
:-- | :--
Dokument* | Wählen Sie hier ein cobra-Dokumentenfeld, in dem die E-Rechnung angefügt wird.
Dokumentdatum* | Wählen Sie hier ein cobra-Datumsfeld, in dem das Datum der Generierung der E-Rechnung hinterlegt wird.
Hauptvorlage* | Wählen Sie hier die gewünschte Rechnungsvorlage aus.
Untervorlage* | Wählen Sie hier die Vorlage für Positionen sowie für Zu- und Abschläge aus.

## Verkäufer

<img src="/docs/Verkäufer.webp" alt="Verkäufer"/> 

Feld | Beschreibung 
:-- | :-- |   
Unternehmen* | Geben Sie hier den Namen des Verkäufers ein, mit dem er im Handelsregister eingetragen oder als steuerpflichtige Person registriert ist. 
Adresse* | Geben Sie hier Straße und Hausnummer der Postanschrift des Verkäufers ein.
PLZ* | Geben Sie hier die Postleitzahl der Postanschrift des Verkäufers ein.
Ort* | Geben Sie hier den Ort der Postanschrift des Verkäufers ein.
Land* | Wählen Sie hier das Land der Postanschrift des Verkäufers aus. `ISO 3166-1 alpha-2`
E-Mail* | Geben Sie hier die E-Mail-Adresse der Ansprechperson bei Rückfragen an den Verkäufer ein.
Telefonnummer* | Geben Sie hier die Telefonnummer der Ansprechperson ein.
USt-IdNr* | Geben Sie hier die Umsatzsteuer-Identifikationsnummer (ID) des Verkäufers ein, sofern kein Steuervertreter angegeben wird.
Steuernummer* | Geben Sie hier die Steuernummer oder den eingetragenen Steuerstatus des Verkäufers ein, z. B. die Umsatzsteuerbefreiung.
Ansprechpartner | Geben Sie hier den Namen der Ansprechperson bei Rückfragen an den Verkäufer ein.

> [!NOTE]
> Für Verkäufer-Ansprechpartner können Sie auch den cobra-Benutzernamen verwenden. Stellen Sie sicher, dass die Benutzerverwaltung in cobra entsprechend gepflegt ist. Verwenden Sie hier für den entsprechenden Knopf im Feld.

## Käufer

<img src="/docs/Käufer.png" alt="Käufer"/> 

Feld | Beschreibung 
:-- | :-- | 
Käufer* | Wählen Sie hier die Beziehung zum Käufer aus. 
Unternehmen* | Geben Sie hier den Namen des Käufers ein, mit dem er im Handelsregister eingetragen oder als steuerpflichtige Person registriert ist.
Adresse* | Geben Sie hier Straße und Hausnummer der Postanschrift des Käufers ein.
PLZ* | Geben Sie hier die Postleitzahl der Postanschrift des Käufers ein.
Ort* | Geben Sie hier den Ort der Postanschrift des Käufers ein.
Land* | Wählen Sie hier das Land der Postanschrift des Käufers aus. `ISO 3166-1 alpha-2`
E-Mail* | Geben Sie hier die E-Mail-Adresse des Käufers ein.
Ansprechpartner | Geben Sie hier den Namen der Ansprechperson bei Rückfragen an den Käufer ein.
Telefonnummer | Geben Sie hier die Telefonnummer der Ansprechperson ein.
USt-IdNr | Geben Sie hier die Umsatzsteuer-Identifikationsnummer des Käufers ein.
Leitweg-ID | Geben Sie hier die Leitweg-ID des Käufers ein. Pflicht für behördliche Rechnungen, bei B2B Rechnungen optional.
XRechnung | Wählen Sie hier, wenn anstelle eines PDFs nur ein reines XML-Format generiert werden soll, das den Anforderungen der europäischen Norm EN 16931 entspricht.
Rechnungsempfänger | Wählen Sie hier die Beziehung zum Rechnungsempfänger. Die Felder für den Rechnungsempfänger werden anhand der gleichen Konfiguration wie für den Käufer festgelegt. Ist kein Rechnungsempfänger angegeben, wird der Käufer automatisch als Rechnungsempfänger festgelegt.

## Position

<img src="/docs/Position.webp" alt="Position"/> 

Feld | Beschreibung 
:-- | :-- | 
Position* | Wählen Sie hier Ihre Positionstabelle.
Sortierung* | Wählen Sie hier ein Feld für die Sortierung aus.
Verknüpfung* | Wählen Sie hier die Beziehung zur Positionstabelle. 
Menge* | Geben Sie hier die Menge des in Rechnung gestellten Artikels ein.
Bezeichnung* | Geben Sie hier die Bezeichnung des in Rechnung gestellten Artikels ein.
Einzelpreis* | Geben Sie hier den Einzelpreis für den Artikel ohne Umsatzsteuer ein.
Artikel-Nr | Geben Sie hier die Kennung des in Rechnung gestellten Artikels ein, die vom Verkäufer zugewiesen wird.
Detailbeschreibung | Geben Sie hier eine detaillierte Beschreibung des in Rechnung gestellten Artikels ein.
USt | Wählen Sie hier die für den in Rechnung gestellten Artikel geltende Umsatzsteuerkategorie aus.
Reverse-Charge | Geben Sie an, ob es sich um eine Reverse-Charge handelt.
Nachlassprozent | Geben Sie hier den prozentualen Nachlass ein.
Nachlassbetrag | Geben Sie hier den Nachlassbetrag (ohne Umsatzsteuer) ein, der u. a. des Prozentsatzes vom Positionsbetrag abgezogen wird.
Nachlassgrund | Geben Sie hier den Grund für den Nachlass ein. 
 
## Zu- und Abschlag

<img src="/docs/Abschlag.webp" alt="Zu- und Abschlag"/> 

Feld | Beschreibung 
:-- | :-- | 
Tabelle | Wählen Sie hier Ihre Tabelle für Zu- und Abschläge auf Rechnungsebene.
Sortierung | Wählen Sie hier ein Feld für die Sortierung aus.
Verknüpfung | Wählen Sie hier die Beziehung zur Tabelle für Zu- und Abschläge. 
Grund | Geben Sie hier den Grund für den Zu- oder Abschlag ein.
Betrag | Geben Sie hier den Betrag (ohne Umsatzsteuer) ein, der u. a. des Prozentsatzes dem Gesamtrechnungsbetrag als Zu- oder Abschlag hinzugefügt wird. 
USt | Geben Sie hier den Umsatzsteuersatz in Prozent ein, der für den Zu- oder Abschlag gilt.
Prozentsatz | Geben Sie hier den prozentualen Zu- oder Abschlag ein.
Grundbetrag | Geben Sie hier den Grundbetrag ein, der unter Anwendung des Prozentsatzes des Zu- oder Abschlag den Betrag ergibt. 
Abschlag | Wählen Sie hier, ob es sich um einen Abschlag handelt, andernfalls ist es ein Zuschlag.
Reverse-Charge | Geben Sie an, ob es sich um eine Reverse-Charge handelt.


## Zahlungsdaten

<img src="/docs/Zahlungsdaten.png" alt="Zahlungsdaten"/> 

Feld | Beschreibung 
:-- | :-- | 
Zahlungsart* | Wählen Sie hier die Zahlungsart.
Währung* | Wählen Sie die Währung aus, in der alle Rechnungsbeträge angegeben werden. `ISO 4217`
Kontoinhaber* | Geben Sie hier den Namen des bei einem Zahlungsdienstleister geführten Zahlungskontos an, auf das die Zahlung erfolgen sollte.
IBAN* | Geben Sie hier die IBAN des Zahlungsempfängers ein.
BIC* | Geben Sie hier die BIC des Geldinstituts ein.
Mandatsreferenz* | Geben Sie hier die Mandatsreferenznummer ein, die dem Käufer vom Verkäufer zugeteilt wird.
Gläubiger-ID* | Geben Sie hier die Gläubiger-Identifikationsnummer ein, die dem Verkäufer von der Deutschen Bundesbank zugeteilt wird. 
Gläubiger-IBAN* | Geben Sie die IBAN des Gläubigers ein.
Gläubiger-BIC* | Geben Sie die BIC des Gläubigers ein.
Verwendungszweck | Geben Sie hier den Verwendungszweck ein, der vom Käufer bei der Zahlung angegeben werden soll.
Zahlungsbedingungen | Geben Sie hier die Zahlungskonditionen ein.
Vorauszahlung | Geben Sie hier die Summe der bereits gezahlten Beträge ein.

## Filter

<img src="/docs/Filter.png" alt="Filter"/> 

Hier können Sie einen frei wählbaren Filter konfigurieren.

## Kontakteintrag

<img src="/docs/Kontakteintrag.png" alt="Kontakteintrag"/> 

Feld | Beschreibung 
:-- | :-- | 
Kontakt anlegen | Soll automatisch ein Kontakt angelegt werden, klicken Sie die Option `Kontakt anlegen` an.
Art* | Wählen Sie hier die Art des Kontakteintrags
Gruppe* | Wählen Sie hier die Gruppe des Kontakteintrags
Bemerkung | Hier können Sie eine Bemerkung zum Kontakteintrag hinzufügen. Sie können dafür alle Platzhalter für Rechnung, Adresse und System verwenden. Wenn das Feld leer bleibt, wird automatisch der Name des Formats sowie die Rechnungsnummer eingetragen. 

## Datenschutz

> [!NOTE]
> Der Menüpunkt `Datenschutz` wird nur angezeigt, wenn die Abfrage der Personenbezogenen Daten aktiviert ist. Hier können Sie einen festen Wert hinterlegen. Wenn kein Wert hinterlegt wird, erfolgt vor jeder Generierung eine Abfrage zur Datenweitergabe.
> 
> Weitere Information zu Datenschutz und [Personenbezogenen Daten](https://systemverwalter.cobra-hilfe.de//docs/datenschutz) finden Sie hier.

<img src="/docs/Datenschutz.png" alt="Datenschutz"/> 

Feld | Beschreibung 
:-- | :-- | 
Weitergabeziele | Interne Verarbeitung, Weitergabe an Dritte, Weitergabe an Drittland
Empfänger | Wird bei Interner Verarbeitung nicht angezeigt. 
Land | Wird nur bei Drittland angezeigt. 
Grund | Wird immer angezeigt. 

##

[Nächste](./Viewer.md) 
