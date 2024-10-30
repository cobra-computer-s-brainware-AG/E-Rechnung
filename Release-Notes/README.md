# Release Notes | E-Rechnung

> [!NOTE]
> Die Anleitung für das Update finden Sie [hier](/Erste-Schritte/Update.md)

## Beta 9

* ### NEU: Abrechnungszeitraum
  In den Einstellungen unter `Allgemein` kann nun ein fixes Datum oder ein Zeitraum konfiguriert werden. `#23`

* ### NEU: Sortierung der Positionstabelle
  In den Einstellungen unter "Position" kann die Sortierung der Positionstabelle konfiguriert werden. `#40`
 
* ### Diverse Bugfixes
  Der fehlerhafte Platzhalter wurde in der Techlify-Positionsvorlage korrigiert.

  Der Ansprechpartner Button wurde in den Einstellungen optimiert. `#42`

  Datensatz wird vor der Generierung aktualisiert. `#43`

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
 
* ### Diverse Bugfixes
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
