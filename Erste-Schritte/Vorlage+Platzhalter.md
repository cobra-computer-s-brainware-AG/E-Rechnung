Erste Schritte

# Vorlage & Platzhalter

Für die Generierung der E-Rechnung stehen Ihnen drei Tabellen zur Verfügung: Adressen, Rechnung und Position. 
Die Rechnungstabelle dient als Ausgangstabelle. An diese werden die Elterntabelle (Adressen) und die Kindtabelle  (Positionen) angehängt. 

Die Elterntabelle besteht aus einem einzelnen Datensatz, der die Rechnungsadresse abbildet. 

Die Kindtabelle hingegen kann mehrere Datensätze enthalten, die jeweils einzelnen Positionen der zugehörigen Rechnungstabelle darstellen, die in der Rechnung aufgeführt sind. 

<p align="center">
<img src="/docs/ERD-light.webp#gh-light-mode-only" alt="ERD" Height="300" />
</p>

## Vorlage

Zur Erstellung einer E-Rechnung werden zwei Word-Vorlagen benötigt: eine `Hauptvorlage`, die die Tabellen Adressen und Rechnung enthält, sowie eine `Untervorlage`, die für die Tabelle Positionen verwendet wird.   
Für jeden Datensatz der Kind-Tabelle wird automatisch eine Tabelle basierend auf der Untervorlage generiert und mit dem Präfix `Tabellenname` in die Hauptvorlage eingefügt.   
Die `Zu- und Abschläge` werden ebenfalls in der Untervorlage als separate Tabelle definiert und mit dem Präfix Tabellenname in die Hauptvorlage eingebunden.   
Die `Umsatzsteuer` wird in der Hauptvorlage automatisch für jeden Steuerschlüssel ergänzt. 

<p align="center">
<img src="/docs/Template-ligh.webp#gh-light-mode-only" alt="Template" Height="400" /> 
</p>

## Platzhalter

Die Platzhalter werden wie folgt aufgebaut: Sie setzen sich aus einem Präfix, dem `Tabellenname`, und einem Suffix, dem `Feldname`, zusammen. Zum Beispiel: {Adressen.Firma}, {Rechnung.Rechnungsnummer}, {Position.Artikel} usw.

Zusätzlich zu den cobra-Seriendruckfeldern stehen weitere Standardplatzhalter zur Verfügung:

### Rechnungstabelle

Platzhalter | Wert
:-- | :--
{CurUserName} | cobra Benutzername
{CurUserShortName} | cobra Kürzel
{Unternehmen} | Unternehmen
{Ansprechpartner} | Ansprechpartner
{Adresse} | Adresse
{PLZ} | PLZ
{Ort} | Ort
{Telefonnummer} | Telefonnummer
{E-Mail} | E-Mail
{IBAN} | IBAN
{BIC} | BIC
{Ust-IdNr} | Ust-IdNr
{Steuernummer} | Steuernummer
{Währung} | Währung
{Warenwert} | Positionssumme
{Zuschlagwert} | Zuschlagsumme
{Abschlagwert} | Abschlagsumme
{Zu- und Abschlagwert} | Zu- und Abschlägesumme
{Netto} | Rechnungssumme ohne USt.
{USt} | Steuerbetrag
{Brutto} | Bruttosumme
{QR} | GiroCode 2x2 cm 

### Umsatzsteuer

> [!NOTE]
> Die Umsatzsteuer wird in der Hauptvorlage automatisch untereinander erweitert.
 
Platzhalter  | Wert
:-- | :--
{USt%} | Steuersatz in Prozent
{Basisbetrag} | Basisbetrag
{Steuerbetrag} | Steuerbetrag

### Positionstabelle
  
Platzhalter  | Wert
:-- | :--
{Pos} | Positionsnummer
{Menge} | Menge 
{Mengeneinheit} | Mengeneinheit
{Artikel-Nr} | Artikel-Nr
{Bezeichnung} | Bezeichnung
{Detailbeschreibung} | Detailbeschreibung
{Einzelpreis} | Einzelpreis
{Gesamtpreis} | Gesamtpreis
{USt%} | Steuersatz in Prozent
{Rabatt%} | Rabatt in Prozent
{Rabatt} | Rabattbetrag 

### Zu- und Abschlagtabelle

Platzhalter  | Wert
:-- | :-- 
{Grund} | Grund
{Prozentsatz} | Prozentsatz
{Basisbetrag} | Basisbetrag
{Betrag} | Betrag
{USt%} | Steuersatz in Prozent

##

[Nächste](./Installation.md) 
