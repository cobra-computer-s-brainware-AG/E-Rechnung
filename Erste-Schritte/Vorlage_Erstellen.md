Erste Schritte

# Word-Vorlage erstellen

In diesem Kapitel wird beschrieben, wie Sie die Word-Vorlage erstellen und die Platzhalter für die personalisierte E-Rechnung einfügen.
 
- Erstellen Sie mit `Microsoft Word` eine neue Hauptvorlage und Untervorlage.
- Fügen Sie in die Hauptvorlage und Untervorlage Ihre Texte und Platzahlter hinzu.
- Speichern Sie die Hauptvorlage und Untervorlage als `Word-Vorlage` mit der Endung `*.dotx`.
  
## Platzhalter in die Hauptvorlage einfügen
In der Hauptvorlage können Sie die `Systemplatzhalter` als auch die `cobra Seriendruckfelder` für die Tabellen `Adresse` und `Rechnung` hinzufügen.
Die Platzhalter für die cobra Seriendruckfelder werden wie folgt aufgebaut: Sie setzen sich aus einem `Präfix`, dem cobra-Tabellennamen, und einem `Suffix`, dem Feldname, zusammen.
 
Die Tabellennamen finden Sie in den Einstellungen im gewünschten Format. Der Präfix für Adresse ist `Adressen`.
  
<img src="/docs/PräfixRechnung.webp" alt="Präfix Rechnung"/> 

Fügen Sie nun den Tabellennamen zusammen mit dem Feldnamen in Ihre Hauptvorlage ein. 

Zum Beispiel: `{Adressen.Adresskopf}`, `{Adressen.Briefanrede}`, `{E-Rechnung.Rechnungsdatum}`, `{E-Rechnung.Lieferdatum}` usw.

<img src="/docs/Hauptvorlage.webp" alt="Hauptvorlage Beispiel"/> 

> [!NOTE]
> Die Systemplatzahlter finden Sie [hier](/Erste-Schritte/Vorlage+Platzhalter.md#platzhalter)



## Platzhalter in die Untervorlage einfügen
In der Untervorlage können Sie die `Systemplatzhalter` als auch die `cobra Seriendruckfelder` für die Tabellen `Position` und `ZU- und Abschlag` hinzufügen.
Die Platzhalter für die cobra Seriendruckfelder werden wie folgt aufgebaut: Sie setzen sich aus einem `Präfix`, dem cobra-Tabellennamen, und einem `Suffix`, dem Feldname, zusammen.

Die Tabellennamen finden Sie in den Einstellungen im gewünschten Format. 

<img src="/docs/PräfixPosition.webp" alt="Präfix Position"/> 

<img src="/docs/PräfixAbschlag.webp" alt="Präfix Abschlag"/>

> [!IMPORTANT]
> Die Platzhalter in der Untervorlage müssen innerhalb einer Tabelle eingefügt werden.

Fügen Sie nun den Tabellennamen zusammen mit dem Feldnamen in Ihre Untervorlage ein.

Zum Beispiel: `{E-Position.Detailbeschreibung}`, `{Zu- und Abschlag.Grund}` usw.

<img src="/docs/Untervorlage.webp" alt="Untervorlage Beispiel"/>  

> [!NOTE]
> Die Systemplatzahlter finden Sie [hier](/Erste-Schritte/Vorlage+Platzhalter.md#platzhalter)



## Untervorlage in Hauptvorlage einbinden

<p align="center">
<img src="/docs/Subtemplate-light.webp" alt="Subtemplate" Height="400" /> 
</p>

Die Positionstabelle sowie die Zu- und Abschlagtabelle werden nur mit dem `Präfix` des cobra-Tabellennamens in die Hauptvorlage eingebunden.
 
<img src="/docs/HauptvorlageUntervoralge.webp" alt="Untervorlage in Hauptvorlage"/>
 
> [!TIP]
> Verbinden Sie hierfür alle Zellen in einer Zeile.


## Umsatzsteuer in Hauptvorlage einbinden

<p align="center">
<img src="/docs/Taxtemplate-light.webp" alt="Taxtemplate" Height="400" /> 
</p>

Die Umsatzsteuer wird in der Hauptvorlage automatisch für jeden Steuerschlüssel ergänzt. 

Fügen Sie dafür die entsprechenden Systemplatzhalter in Ihre Hauptvorlage.
 
<img src="/docs/HauptvorlageUmstzstuer.webp" alt="Umsatzsteuer in Hauptvorlage"/> 
  
> [!IMPORTANT]
> Die Platzhalter für Umsatzsteuer müssen innerhalb einer Tabelle eingefügt werden.

> [!NOTE]
> Die Systemplatzahlter finden Sie [hier](/Erste-Schritte/Vorlage+Platzhalter.md#platzhalter)
 

## 
 
[Nächste](./Installation.md)
 
