# <a name="installing-the-custom-learning-solution-webpart"></a>Installieren der benutzerdefiniertes Lösung Webpart lernen

## <a name="prerequisites-for-a-tenant-wide-installation"></a>Erforderliche Komponenten für eine gesamte Mandanten-installation

- Um die benutzerdefinierte Learning-Webpart für Ihre gesamte Mandanten zu installieren, müssen Sie Office 365-Administratorberechtigungen verfügen.  Wenn Sie nicht über diese Berechtigungen verfügen, die können Sie gemeinsam mit dem Office 365-Administrator oder installieren das Webpart für eine einzelne Websitesammlung.
- Sie oder Ihr Office 365-Administrator muss Setup und konfiguriert einen Mandanten geltende [App-Katalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) oder [Site Collection App-Katalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog), um das Webpart empfangen.]
- Wir unterstützen nur SharePoint Online. Das Webpart wird nicht unterstützt für die Installation auf eine beliebige Version von SharePoint lokal.

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a>Hinzufügen des benutzerdefinierte Learning-Webparts zu Ihrem Mandanten 

1. Laden Sie das benutzerdefinierte Learning-Webpart, und speichern Sie sie auf Ihrem lokalen Laufwerk.  Dieser Datei lautet "ms-benutzerdefinierte-learning.sppkg".  Ändern Sie den Namen oder die Suffix der Datei nicht. 
2. Navigieren Sie zu der [Office 365-Verwaltungsportal](https://admin.microsoft.com/AdminPortal/Home#/homepage) für Ihre Mandanten
3. Wählen Sie im linken Navigationsbereich Admin Center, SharePoint aus. Dadurch wird eine neue Registerkarte, und wählen Sie Apps In the SharePoint Admin Center, App-Katalog, Apps für SharePoint geöffnet. 
4. Aktivieren Sie das Webpart hochladen und wählen Sie die heruntergeladene Datei "ms-benutzerdefinierte-learning.sppkg"
5. Für diese Mandanten geltende Installation das Kontrollkästchen Sie neben "Diese Lösung für alle befindet sich in der Organisation verfügbar machen."  

![Bereitstellen der Lösung](media/trustapp_sm.png)


## <a name="add-the-customer-learning-webpart-to-a-sharepoint-online-page"></a>Hinzufügen des Kunden Learning-Webparts zu einer SharePoint Online-Seite

Nach der Installation benutzerdefinierte Learning in Ihrem Mandanten können Sie das Webpart zu einer SharePoint-Seite hinzufügen. Wenn Sie dies tun, ist plötzlich Office 365-Schulung für Sie verfügbar. 

1. Fügen Sie die benutzerdefinierte Learning-Webpart in ein Layout mit voller Breite Spalten hinzu:

![SharePoint-Seitenlayout](media/clo365fullcolumnwidth.png)

2. Wählen Sie im Abschnitt hinzufügen, und wählen Sie dann volle Breitenspalte, in der SharePoint-Seite.  Sehen Sie die folgende Meldung angezeigt:

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. Wählen Sie Microsoft Learning.  Sie sollten nun Folgendes angezeigt: 

![Benutzerdefinierte Webpart lernen](media/clo365addwebpart.png)

 Sie können nun auf die Kacheln zum Untersuchen des Standardinhalts in der Projektmappe enthaltenen klicken.  

## <a name="next-steps"></a>Weitere Schritte
- Verwenden Sie das [Standardkonto](webpartcontent.md) in das Webpart aus.
- [Anpassen](customization.md) der Schulung Erfahrung für Ihre Organisation.
- [Bessere Akzeptanz](driveadoption.md) der Schulung Lösung ist.

