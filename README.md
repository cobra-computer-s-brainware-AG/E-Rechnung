# cobra E-Rechnung
 
cobra CRM AddOn zur Generierung von E-Rechnungen

Erstellen Sie mit wenigen Klicks gesetzlich konforme E-Rechnungen direkt aus Ihrem cobra CRM-System. 
Versenden Sie die E-Rechnungen digital als E-Mail oder Serien-E-Mail an Ihre Kunden. 
So sind Sie bestens vorbereitet auf die kommenden gesetzlichen Änderungen.

Bleiben Sie konform und sparen Sie Zeit mit unserer benutzerfreundlichen und effizienten Lösung!
 
## Kompatibel

| latest version | CRM BI | CRM PRO | CRM PLUS | ADRESS PLUS |
| :-- | :--: | :--: | :--: | :--: |
| Viewer | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
| E-Rechnung | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark:* | :x: |

\* CRM PLUS unterstützt keine freien Tabellen, keine Beziehungsfelder, keine Kopierregel ect. die vorteilhaft sein könnten, zb. für Artikelstamm.

## Kurzanleitung 

### Installation 

Die E-Rechnung-Erweiterung wird in `2 Installationen` unterteilt. Die Netzwerk-Installation und die Client-Installation. Die Netzwerkinstallation stellt sicher, dass alle Clients dieselbe Version verwenden.

1. Installieren Sie die E-Rechnung-Erweiterung `E-Rechnung.Installer.msi` in Ihr cobra Systemverzeichnis.
   <img src="docs/System_Installation.png" alt="Installation"/>
2. Installieren Sie danach das ClientSetup `E-Rechnung.ClientSetup.64.msi` auf dem gewünschten Client.
   <img src="docs/Installation.png" alt="Installation"/> 
4. Nach erfolgreicher Installation erscheint in Ihrem cobra CRM der Reiter `E-Rechnung`.
   <img src="docs/Ribbon.png" alt="Ribbon"/> 
5. Für Testzwecke empfehlen wir, die automatische Generierung der Datenbankstruktur zu nutzen, bevor Sie mit der individuellen Konfiguration beginnen. Dies wird beim ersten Klick auf `Einstellungen` angeboten.
   <img src="docs/Datenbankstruktur.png" alt="Datenbankstruktur" /> 
   - Zusätzlich zur Datenbankstruktur werden Demodaten, Demo-Format, Demoansicht und ein Demo-Serien-E-Mail-Format angelegt. So können Sie direkt mit dem Testen beginnen. 
6. Nach der Generierung müssen Sie cobra neu starten.
7. Abschließend konfigurieren Sie das Dokumentenfeld in der Rechnungstabelle gemäß Ihren Schlagwörtern.
   - Optional können Sie Eingabemasken, Ansichten und Anzeigeformat an Ihre Bedürfnisse anpassen.


### Zusätzliche Informationen:

#### Vorlage
Die Haupt- und Untervorlage für die Demo Rechnung finden Sie im cobra-Systemverzeichnis unter `System\Schnittstellen\E-Rechnung`. Diese können Sie individuell gestalten. Ihnen stehen alle Seriendruckfelder und Textbausteine aus Ihrem cobra CRM-System für die Tabellen Adresse, Rechnung und Position zur Verfügung.

#### Serienrechnung 
Nach jeder Generierung wird das Feld `Dokumentdatum` mit dem Generierungsdatum befüllt. Wenn dieses Feld ausgefüllt ist, kann keine neue Serienrechnung erstellt werden.

#### Serien-E-Mail 
Verwenden Sie den Standardfilter `Letzte Serienrechnung`, um Ihre zuletzt erstellten Serienrechnungen zu filtern. Alternativ können Sie mit dem freien Filter Ihre eigene Logik verwenden.

## Voralge & Platzhalter
Für die Generierung der E-Rechnung stehen Ihnen drei Tabellen zur Verfügung: Adressen, Rechnung und Position. 
Die Rechnungstabelle dient als Ausgangstabelle. An diese werden die Eltern-Tabelle (Adressen) und die Kind-Tabelle (Positionen) angehängt. 

Die Eltern-Tabelle besteht aus einem einzelnen Datensatz, der die Rechnungsadresse abbildet. 

Die Kind-Tabelle hingegen kann mehrere Datensätze enthalten, die jeweils einzelne Positionen zur zugehörigen Rechnungstabelle darstellen, die in der Rechnung aufgeführt sind. 

<p align="center">
<img src="docs/ERD-light.svg#gh-light-mode-only" alt="ERD" Height="300" />
<img src="docs/ERD-dark.svg#gh-dark-mode-only" alt="ERD" Height="300" />
</p>

Zur Erstellung einer E-Rechnung werden zwei Word-Vorlagen benötigt: Eine Hauptvorlage, die die Adress- und Rechnungstabellen enthält, sowie eine Untervorlage, die für die Positionstabelle verwendet wird.  
Für jeden Kind-Datensatz wird automatisch eine Tabelle basierend auf der Untervorlage generiert. Diese wird mit dem Präfix `Tabellenname` in die Hauptvorlage eingefügt.  
Die `Umsatzsteuer` wird in der Hauptvorlage automatisch für jeden Steuerschlüssel erweitert.  

<p align="center">
<img src="docs/Template-ligh.svgt#gh-light-mode-only" alt="Template" Height="400" />
<img src="docs/Template-dark.svg#gh-dark-mode-only" alt="Template" Height="400" />
</p>

### Platzhalter
Die Platzhalter werden wie folgt aufgebaut: Sie setzen sich aus einem Präfix, dem `Tabellenname`, und einem Suffix, dem `Feldname`, zusammen. Zum Beispiel: {Adressen.Firma}, {Rechnung.Rechnungsnummer}, {Position.Artikel} usw.

Zusätzlich zu den cobra-Seriendruckfeldern stehen weitere Standardplatzhalter zur Verfügung:

### Rechnungstabelle

Platzhalter | Wert
:-- | :--
{CurUserName} | cobra Bentuzername
{CurUserShortName} | cobra Kürzel
{Unternehmen} | 
{Adresse} | 
{PLZ} | 
{Ort} | 
{Telefonnummer} | 
{E-Mail} | 
{IBAN} | 
{BIC} | 
{Ust-IdNr} | 
{Währung} | 
{Warenwert} | 
{Netto} | 
{USt} | 
{Brutto} | 
{QR} | GiroCode 2x2cm 

### Umsatzsteuer

> [!NOTE]
> Die Umsatzsteuer wird in der Hauptvorlage automatisch untereinander erweitert.
 
Platzhalter  | Wert
:-- | :--
{USt%} | 
{Basisbetrag} | 
{Steuerbetrag} | 

### Positionstabelle
  
Platzhalter  | Wert
:-- | :--
{Pos} | 
{Menge} | 
{Mengeneinheit} | 
{Artikel-Nr} | 
{Bezeichnung} | 
{Detailbeschreibung} | 
{Einzelpreis} | 
{Gesamtpreis} | 
{USt%} | 
{Rabatt%} | 
{Rabatt} | 
