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
|  | Leitweg-ID | Text 
|  | XRechnung | Ja/Nein

### Rechnung

Die Rechnungstabelle wird für die Verwaltung der Rechnung benötigt.

Pflicht  | Feldname | Feldtyp |
:--: | :-- | :-- |
| :heavy_exclamation_mark: | Käufer (Adresse) | SuperId, FK
| :heavy_exclamation_mark: | Rechnungsnummer | Zahl, Zähler, ID, Text, Virtuell
| :heavy_exclamation_mark: | Rechnungsdatum | Datum 
| :heavy_exclamation_mark: | Lieferdatum | Datum 
| :heavy_exclamation_mark: | Dokument | Dokument 
| :heavy_exclamation_mark: | Dokumentdatum | Datum 
| | Fälligkeitsdatum | Datum 
| | Verwendungszweck | Text
| | Zahlungsbedingungen | Text
| | Vorauszahlung | Zahl, Währung
| | Projektkennung | Text, Zahl
| | Vertragsnummer | Text, Zahl
| | Bestellnummer | Text, Zahl
| | Bemerkung | Bemerkung 
| | Rechnungsempfänger (Adresse) | SuperId, FK

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
| | Nachlassprozent | Zahl 
| | Nachlassbetrag | Zahl, Währung  
| | Nachlassgrund | Text 
  
##

[Nächste](./Vorlage+Platzhalter.md) 
