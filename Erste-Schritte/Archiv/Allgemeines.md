Erste Schritte

# Allgemeines

Ihre E-Rechnung in korrekter Form erstellt – ganz einfach mit cobra.
 
## Kompatibel

| latest version | CRM BI | CRM PRO | CRM PLUS | ADRESS PLUS |
| :-- | :--: | :--: | :--: | :--: |
| Viewer | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| E-Rechnung | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark:* | :x: |

> [!NOTE]
> CRM PLUS unterstützt keine freien Tabellen, keine Beziehungsfelder, keine Kopierregel ect. die vorteilhaft sein könnten, zb. für Artikelstamm.

## Datenbankstruktur

Für die Inbetriebnahme der E-Rechnung sind folgende Tabellen und Felder erforderlich. Die Pflichtfelder sind entsprechend markiert.
   
### Adressen

Die Adresstabelle wird für die Rechnungsadresse benötigt.

Pflicht  | Feldname | Feldtyp |
:--: | :-- | :-- |
| :heavy_exclamation_mark: | Unternehmen | Firma
| :heavy_exclamation_mark: | Adresse | Straße 
| :heavy_exclamation_mark: | PLZ | PLZ
| :heavy_exclamation_mark: | Ort | Ort
| :heavy_exclamation_mark: | Land | Land
| :heavy_exclamation_mark: | E-Mail | E-Mail
|  | Ansprechpartner | Vorname, Nachname, Virtuell
|  | Telefonnummer  | Telefon
|  | USt-IdNr | Text 
|  | Leitweg-ID | Text 
|  | XRechnung | Ja/Nein
|  | Mandatsreferenz | Text 
|  | Gläubiger-ID | Text 
|  | Gläubiger-IBAN | IBAN 
|  | Gläubiger-BIC | BIC 

### Rechnung

Die Rechnungstabelle wird für die Verwaltung der Rechnung benötigt.

Pflicht  | Feldname | Feldtyp |
:--: | :-- | :-- |
| :heavy_exclamation_mark: | Verknüpfung zur Adresse (Käufer) | SuperId, FK
| :heavy_exclamation_mark: | Rechnungsnummer | Zahl, Zähler, ID, Text, Virtuell
| :heavy_exclamation_mark: | Rechnungsdatum | Datum 
| :heavy_exclamation_mark: | Liefer-/Leistungsdatum | Datum 
| :heavy_exclamation_mark: |  Dokument | Dokument 
| :heavy_exclamation_mark: |  Dokumentdatum | Datum 
| :heavy_exclamation_mark: |  E-Mail für Versand | E-Mail
| | Abrechnungszeitraum Von | Datum 
| | Abrechnungszeitraum Bis | Datum 
| | Fälligkeitsdatum | Datum 
| | Verwendungszweck | Text
| | Zahlungsbedingungen | Text
| | Vorauszahlung | Zahl, Währung
| | Projektkennung | Text, Zahl
| | Vertragsnummer | Text, Zahl
| | Bestellnummer | Text, Zahl
| | Bemerkung | Bemerkung 
| * | Verknüpfung zur Adresse (Rechnungsempfänger) | FK

> [!NOTE]
> *nicht in CRM PLUS möglich

### Position

Die Positionstabelle wird für die in Rechnung gestellten Leistungen benötigt.

Pflicht  | Feldname | Feldtyp |
:--: | :-- | :-- |
| :heavy_exclamation_mark: | Verknüpfung zur Rechnung | SuperId, FK
| :heavy_exclamation_mark: | Menge | Zahl, Rechenfeld
| :heavy_exclamation_mark: | Bezeichnung | Text 
| :heavy_exclamation_mark: | Einzelpreis | Zahl, Währung 
| | Artikel-Nr | Text 
| | Detailbeschreibung | Text, Bemerkung
| | USt | Zahl 
| | Reverse-Charge | Ja/Nein
| | Prozent | Zahl 
| | Betrag | Zahl, Währung, Rechenfeld
| | Grund | Text  

### Zu- und Abschlag

Die Zu- und Abschlagtabelle wird zur Verwaltung von Zu- und Abschlägen auf Rechnungsebene verwendet, zb. für Lieferpauschalen oder Kopfrabatt. 

> [!NOTE]
> Diese Tabelle ist optional und für dieses Modul nicht zwingend erforderlich.

Pflicht  | Feldname | Feldtyp |
:--: | :-- | :-- |
| :heavy_exclamation_mark: | Verknüpfung zur Rechnung | SuperId, FK
| :heavy_exclamation_mark: | Grund | Text 
| :heavy_exclamation_mark: | Betrag | Zahl, Währung, Rechenfeld
| | USt | Zahl 
| | Prozentsaatz | Zahl
| | Grundbetrag | Zahl, Währung, Rechenfeld
| | Abschlag | Ja/Nein
| | Reverse-Charge | Ja/Nein

##

[Nächste](./Vorlage+Platzhalter.md) 
