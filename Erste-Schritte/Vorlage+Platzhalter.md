Erste Schritte

# Vorlage & Platzhalter

Für die Generierung der E-Rechnung stehen Ihnen drei Tabellen zur Verfügung: Adressen, Rechnung und Position. 
Die Rechnungstabelle dient als Ausgangstabelle. An diese werden die Elterntabelle (Adressen) und die Kindtabelle  (Positionen) angehängt. 

Die Elterntabelle besteht aus einem einzelnen Datensatz, der die Rechnungsadresse abbildet. 

Die Kindtabelle hingegen kann mehrere Datensätze enthalten, die jeweils einzelnen Positionen der zugehörigen Rechnungstabelle darstellen, die in der Rechnung aufgeführt sind. 

<p align="center">
<img src="/docs/ERD-light.svg#gh-light-mode-only" alt="ERD" Height="300" />
<img src="/docs/ERD-dark.svg#gh-dark-mode-only" alt="ERD" Height="300" />
</p>

## Vorlage

Zur Erstellung einer E-Rechnung werden zwei Word-Vorlagen benötigt: Eine Hauptvorlage, die die Adress- und Rechnungstabellen enthält, sowie eine Untervorlage, die für die Positionstabelle verwendet wird.  
Für jeden Kind-Datensatz wird automatisch eine Tabelle basierend auf der Untervorlage generiert. Diese wird mit dem Präfix `Tabellenname` in die Hauptvorlage eingefügt.  
Die `Umsatzsteuer` wird in der Hauptvorlage automatisch für jeden Steuerschlüssel erweitert.  

<p align="center">
<img src="/docs/Template-ligh.svgt#gh-light-mode-only" alt="Template" Height="400" />
<img src="/docs/Template-dark.svg#gh-dark-mode-only" alt="Template" Height="400" />
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
{Zuschlagwert} | :new: Zuschlagsumme
{Abschlagwert} | :new: Abschlagsumme
{Zu- und Abschlagwert} | :new: Zu- und Abschlägesumme
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
{Grund} | Grund für den Zu- oder Abschlag
{Prozentsatz} | Prozentsatz für den Zu- oder Abschlag, wird auf den Basisbetrag angewendet
{Basisbetrag} | Basisbetrag zur Berechnung des Prozentsatzes 
{Betrag} | Endbetrag des Zu- oder Abschlags (z.B. berechnet aus Basisbetrag und Prozentsatz)
{USt%} | Steuersatz in Prozent

##

[Nächste](./Installation.md) 
