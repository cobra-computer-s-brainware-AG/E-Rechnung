# Release Notes | E-Rechnung

> [!NOTE]
> Die Anleitung für das Update finden Sie [hier](/Erste-Schritte/Update.md)

## Beta 8

* ### NEU: Variable für Verkäufer-Ansprechperson
  In den Einstellungen unter `Verkäufer` kann nun auch die Variable `{CurUserName}` als cobra-Benutzername verwendet werden. 
 
* ### Diverse Bugfixes
  Beim Erstellen der Kopierregel für die Artikeltabelle kann jetzt auch ein leeres Feld zugewiesen werden.

 
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
