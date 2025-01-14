# Release Notes | E-Rechnung

> [!NOTE]
> Die Anleitung für das Update finden Sie [hier](https://e-rechnung.cobra-hilfe.de/docs/Update)

## RC 1 Patch 3.3

* ### Bugfixes und Diverse

  Bei der Meldung mit dem ISO-3166-1 alpha-2-Länderkürzel wird ein Hyperlink zur Cobra-Hilfe angezeigt. `#108`

  Die Update-Meldung wurde verständlicher formuliert. [#106](https://www.cobrapartner.eu/Forum/Partnerforum76/updatemeldung_topic26058.html#128787)
  
## RC 1 Patch 3.2

* ### Bugfixes und Diverse

  Die Platzhalter für `Zu- und Abschlag` können nun auch in der Word-Vorlage verwendet werden. `#94`

  Die verwendete ZUGFeRD-Version ist in den Einstellungen ersichtlich. `#100`
  
  Der Fehler im ZUGFeRD-Dateinamen wurde behoben. `#101`

  Der Fehler beim Feld `Land` mit dem Wert NULL wurde behoben. `#102`

  Beim automatischen Generieren wird der `INSTEAD_OF_DELETE`-Trigger erstellt. Anschliessend muss cobra neu gestartet werden! `#103`

## RC 1 Patch 3.1

* ### NEU: Weitere Kontakt Felder (CRM PRO/BI)
  In den Einstellungen unter `Kontakteintrag` können weitere Kontaktfelder befüllt werden. Dieses Komfort-Feature steht ausschließlich CRM PRO/BI-Kunden zur Verfügung. `#54`     
  [Weitere Kontakt Felder](/Erste-Schritte/Erweiterte_Einstellungen.md#weitere-kontakt-felder)

* ### NEU: Konfigurierbare Steuerart
  In den Einstellungen unter `Position` oder `Zu- und Abschlag` kann die Steuerart einem Steuersatz zugewiesen werden. Nicht zugeordnete Steuersätze werden automatisch der Steuerart (S) zugewiesen. Der Steuersatz 0 wird der Steuerart (Z) zugeordnet. `#92`     
  [Steuerart Konfigurieren](/Erste-Schritte/Erweiterte_Einstellungen.md#steuerart-konfigurieren)

* ### NEU: Nach Update suchen
  Neu kann über die Schaltfläche `Update suchen` geprüft werden, ob eine neuere Version verfügbar ist. `#94`     
  [Menüband](/Erste-Schritte/Start.md)

* ### Bugfixes und Diverse

  Im Feld `Bemerkung` wird der Standardtext als Platzhalter angezeigt.

  Im Viewer werden jetzt alle Zahlungsbedingungen angezeigt. `#6`

  Im Viewer wurde das Anzeigeformat für die Anzahl korrigiert. `#89`

  Die Übersicht der Serienrechnung wird nach dem Feld `ID` sortiert. `#90`

  Länderkürzel, die nicht dem ISO-Alpha-2-Format entsprechen, können nicht mehr ausgegeben werden. `#91`

  Das Fälligkeitsdatum ist jetzt ein Pflichtfeld.

## RC 1 Patch 2

* ### NEU: cobra-hilfe.de
  Die komplette Anleitung findet Sie neu unter: https://e-rechnung.cobra-hilfe.de

* ### NEU: Disclaimer
  Der Disclaimer in den Einstellungen wurde überarbeitet, und zusätzlich wurde die Rechtschreibung korrigiert.

* ### NEU: Validierung des cobra-Systemverzeichnisses 
  Der `E-Rechnung.Installer.msi` validiert das cobra-Systemverzeichnis. Zusätzlich wird das E-Rechnung-Verzeichnis nur geöffnet, wenn der Loader noch nicht installiert ist. `#85`

* ### NEU: USt heisst jetzt USt in Prozent
  In den Einstellungen unter `Position` sowie `Zu- und Abschlag` wurde das Feld `USt` in `USt in Prozent` umbenannt. `#83`

* ### Bugfixes und Diverse
  Der Fehler im Zusammenhang mit dem Unterdokument wurde behoben. `#77`

  Die Fehlermeldung für die Validierung der Platzhalter wurde angepasst.
 
  In den Einstellungen unter `Dokument` wurden wieder drei Punkte angezeigt.

  Der Fehler bei SetUserWindowSize wird nicht mehr protokolliert.

  Die Serienrechnung ist in der cobra-Demoversion nicht verfügbar.

  Die E-Rechnung-Erweiterung funktioniert nur mit gültiger AGV.

  Das Feld `E-Mail für Versand` muss die gleiche Länge haben wie das E-Mail-Feld in der Adresstabelle. `#80`

  In den Einstellungen wird der logische Name der Tabelle angezeigt. `#81`

  Die IBAN muss eine Länge von mindestens 15 und maximal 31 Zeichen haben.

  Eingabepflichtige Felder werden in der Datenbankstruktur nicht angezeigt. Die Membership und Membershipext wurden korrigiert. `#79`

  Der Fehler mit leeren Datenbanken bei der Generierung der Demodatensätze wurde behoben. `#84`

  Wird in der `Zu- und Abschlagstabelle` kein Wert im Feld `Grundbetrag` angegeben, wird auch kein Wert ausgegeben. `#82`

  Filter wird nicht in den Einstellungen angezeigt wurde behoben. `#88`
  
## RC 1

* ### NEU: Einstellungen Validierung
  In den Einstellungen werden Validierungen direkt über die neuen Badges angezeigt. `#69`
 
* ### Bugfixes und Diverse

  Vertragsnummer und Projektkennung fehlten im XRechnung. `#74` 

  Beim Erstellen der Kopierregel kann der Vorgang abgebrochen werden. Falls die Kopierregel nicht erstellt werden kann, wird ein entsprechender Hinweis ausgegeben. `#72`

  Die Tabelle `Zu- und Abschlag` ist jetzt optional. `#71`

  Die E-Rechnung wird bei einem Update in `Programme und Features` aktualisiert. `#68`

## Beta 10

* ### NEU: cobra 2025
  Die E-Rechnung-Erweiterung ist auch mit `cobra 2025` kompatibel.

* ### NEU: Zugriffsbeschränkung für Einstellungen
  Die Einstellungen sind nur zugänglich, wenn der Benutzer über die Berechtigung für die Datenbankstruktur verfügt. `#60`

* ### NEU: Zu- und Abschläg
  Neu können Zu- und Abschläge auf Rechnungsebene hinzugefügt werden, wofür eine untergeordnete Tabelle zur Rechnung ergänzt wird. Für die Zu- und Abschläge stehen zudem neue Platzhalter in der Wordvorlage zur Verfügung. `#46`     
  [Zu- und Abschläg](/Erste-Schritte/Allgemeines.md#zu--und-abschlag)

* ### NEU: Reverse-Charge
  Neu kann das Reverse-Charge-Verfahren (Umkehr der Steuerschuldnerschaft) sowohl in den `Positionen` als auch bei `Zu- und Abschlägen` angewendet werden. `#45`       
  [Position](/Erste-Schritte/Einstellungen.md#position)
 
* ### NEU: Allgemein heisst jetzt Rechnung
  In den Einstellungen wurde `Allgemein` in `Rechnung` umbenannt.     
  [Rechnung](/Erste-Schritte/Einstellungen.md#Rechnung) 

* ### NEU: E-Mail Feld auf Rechnung
  Um die Rechnung einfacher an die E-Mail-Adresse des Käufers versenden zu können, wird ein neues E-Mail-Feld in der Rechnungstabelle benötigt.
  Beim Erstellen der Rechnung wird die E-Mail-Adresse des Käufers in dieses Feld kopiert.
  Dadurch wird die Konfiguration im Serien-E-Mailer für die Ziel-E-Mail-Adresse vereinfacht, und der Serien-E-Mail-Versand wird auch mit CRM PLUS kompatibel. `#58`      
  [Rechnung](/Erste-Schritte/Einstellungen.md#Rechnung)

* ### NEU: Käufer/Rechnungsempfänger
  Wenn in den Einstellungen unter `Käufer` ein Rechnungsempfänger konfiguriert ist, wird der Käufer bei der Generierung automatisch in das Feld Rechnungsempfänger kopiert, sofern dieses leer ist.
  Im Serien-E-Mailer kann dann die Route zum Rechnungsempfänger gewählt werden, sodass der Kontakteintrag bei der richtigen Adresse abgelegt wird. `#66`

* ### Bugfixes und Diverse
  
  Die Texte für Nachlässe wurden Angepasst. `#59`

  Die Positionen wurden im PDF nicht korrekt sortiert. `#61`

  Das Laden des Datensatzes wurde Optimiert. `#63`

  Leistungsdatum und Abrechnungszeitraum werden bei der Eingabe bereinigt, um unnötige Fehlermeldungen beim Speichern zu vermeiden. `#64`

  Leerer Abrechnungszeitraum wird bei der Generierung besser validiert. `#65`

  Allen Konfigurationsfeldern wurde ein Info-Button hinzugefügt.

  Die Tabelle für Zu- und Abschläge wird bei der automatischen Generierung mit erstellt.

  In den Einstellungen wurde der Filter angepasst, sodass das Beziehungsfeld nicht mehr angezeigt wird.

  Die Datenbankstruktur wird nach der automatischen Generierung automatisch neu geladen.
  

## Beta 9 

* ### NEU: Hinweistext Einstellungen
  Beim Speichern wird ein entsprechender Hinweistext in den Einstellungen angezeigt. 

* ### NEU: USt-ID oder Steuernummer
  In den Einstellungen unter `Verkäufer` ist es nicht mehr erforderlich, dass beide Werte vorhanden sind. `52`      
  [Verkäufer](/Erste-Schritte/Einstellungen.md#verkäufer) 

* ### NEU: Einzelrechnung Aktueller Datensatz
  Eine Einzelrechnung kann nur noch für den aktuellen Datensatz erstellt werden.    
  [Einzelrechnung](/Erste-Schritte/Einzelrechnung.md)

* ### NEU: Rechnungsstellung SEPA Lastschrift 
  In den Einstellungen unter `Zahlungsdaten` kann nun die SEPA-Lastschrift konfiguriert werden.
  Bitte beachten Sie, dass die cobra E-Rechnung Erweiterung keine SEPA-Lastschriftmandate ausführt.
  Die Erweiterung dient ausschließlich der elektronischen Rechnungsstellung und beinhaltet keine Funktionalität für das Einziehen von Zahlungen.`#38`       
  [Zahlungsdaten](/Erste-Schritte/Einstellungen.md#Zahlungsdaten)

* ### NEU: Abrechnungszeitraum
  In den Einstellungen unter `Allgemein` kann nun ein fixes Datum oder ein Zeitraum konfiguriert werden. `#23`

* ### NEU: Sortierung der Positionstabelle
  In den Einstellungen unter `Position` kann die Sortierung der Positionstabelle konfiguriert werden. `#40`

* ### NEU: Hinweis zur Rückdatierung von Rechnungen
  Liegt das Rechnungsdatum nicht in der Zukunft, wird ein entsprechender Hinweis ausgegeben. `#44`
 
* ### Bugfixes und Diverse
  Der fehlerhafte Platzhalter wurde in der Techlify-Positionsvorlage korrigiert.

  Bessere Validierung der Platzhalter. `#41`

  Der Ansprechpartner Button wurde in den Einstellungen optimiert. `#42`

  Datensatz wird vor der Generierung aktualisiert. `#43`

  Der Viewer schließt sich, wenn keine XRechnung ausgewählt wurde. `#47`

  Die Fenstergrösse bei Serienrechnung wird sich nicht mehr automatisch dem Inahlt anpassen. `#50`

  Filter Letzte Serienrechnung anpassung `#51`
 
  Validierung wird beim Speichern Optimiert. `#53`


  
## Beta 8

* ### NEU: Kontakt anlegen 
  In den Einstellungen unter `Kontakteintrag` kann nun festgelegt werden, ob ein Kontakteintrag erstellt werden soll.   
  [Kontakteintrag](/Erste-Schritte/Einstellungen.md#kontakteintrag)

* ### NEU: Erweiterte Feldauswahl für Position
  Für `Menge` steht neu der Typ `Rechenfeld` und für `Detailbeschreibung` der Typ `Bemerkung` zur Auswahl.

* ### NEU: Lieferdatum Pflichtfeld
  Das Feld Lieferdatum wird zum Pflichtfeld.

* ### NEU: Variable für Verkäufer-Ansprechperson
  In den Einstellungen unter `Verkäufer` kann nun auch die Variable `{CurUserName}` als cobra-Benutzername verwendet werden.   
  [Verkäufer](/Erste-Schritte/Einstellungen.md#verkäufer)

* ### NEU: Weitere Systemplatzhalter
  Neu können die Systemplatzhalter `{Steuernummer}` und `{Ansprechpartner}` in der Word-Vorlage verwendet werden. Somit sind alle Verkäufer Felder als Platzhalter verfügbar.   
  [Platzhalter](/Erste-Schritte/Vorlage+Platzhalter.md#platzhalter)
 
* ### Bugfixes und Diverse
  Beim Erstellen der Kopierregel für die Artikeltabelle kann jetzt auch ein leeres Feld zugewiesen werden.

  FK1 Membership wurde korrigiert, und der Filter auf den aktuellen Datensatz wurde entfernt. 
  
  Verbesserte Fehlermeldung, wenn Platzhalter in der Word-Vorlage nicht gefunden werden.

  Das Fälligkeitsdatum ist jetzt kein Pflichtfeld mehr.

  Das Rechnungsdatum wird vor der Generierung validiert.

  UI-Anpassungen in den Einstellungen beim Speichern.

  Einstellungen werden in Adress Plus ausgeblendet.

  QR-Platzhalter aus Kontakteintrag entfernt.

  Im Kontakteintrag lassen sich nun auch Zeilenumbrüche hinzufügen.

  Die Systemmaske wird als Eingabemaske gespeichert, wenn die Datenbankstruktur automatisch generiert wird.
 
## Beta 7 

* ### NEU: Rechnungsempfänger (abweichender Käufer)
  In den Einstellungen unter `Käufer` kann jetzt ein Rechnungsempfänger (abweichender Käufer) konfiguriert werden.  
  [Käufer](/Erste-Schritte/Einstellungen.md#käufer)

* ### NEU: Artikelstamm und Kopierregel
  Ab CRM PRO kann bei der automatischen Datenbankgenerierung die Positionstabelle über ein Beziehungsfeld mit einer Artikeltabelle (Freientabelle) verknüpft werden.  
  Optional kann eine einfache Kopierregel erstellt werden.  
  [automatische Generierung](/Erste-Schritte/Einstellungen.md#automatische-generierung)

* ### Kontakteintrag
  Der Kontakteintrag wird sowohl beim Käufer als auch bei der Rechnungsempfänger hinterlegt.
 
* ### Rechnungsnummer
  In den Einstellungen unter `Allgemein` kann nun auch ein virtuelles Feld für die Rechnungsnummer ausgewählt werden.

* ### Ansprechpartner 
  Der Ansprechpartner muss aus einem Feld des Käufer- oder Rechnungsdatensatzes stammen.

* ### Diverse Bugfixes
