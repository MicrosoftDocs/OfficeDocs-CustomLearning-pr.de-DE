# <a name="installing-the-custom-learning-solution-webpart"></a><span data-ttu-id="8d1b9-101">Installieren der benutzerdefiniertes Lösung Webpart lernen</span><span class="sxs-lookup"><span data-stu-id="8d1b9-101">Installing the Custom Learning Solution Webpart</span></span>

## <a name="prerequisites-for-a-tenant-wide-installation"></a><span data-ttu-id="8d1b9-102">Erforderliche Komponenten für eine gesamte Mandanten-installation</span><span class="sxs-lookup"><span data-stu-id="8d1b9-102">Prerequisites for a tenant-wide installation</span></span>

- <span data-ttu-id="8d1b9-p101">Um die benutzerdefinierte Learning-Webpart für Ihre gesamte Mandanten zu installieren, müssen Sie Office 365-Administratorberechtigungen verfügen.  Wenn Sie nicht über diese Berechtigungen verfügen, die können Sie gemeinsam mit dem Office 365-Administrator oder installieren das Webpart für eine einzelne Websitesammlung.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-p101">To install the Custom Learning webpart for your entire tenant you will need to have Office 365 Administrative permissions.  If you do not have these permissions you can either work with your Office 365 Administrator or install the webpart for an individual site collection.</span></span>
- <span data-ttu-id="8d1b9-105">Sie oder Ihr Office 365-Administrator muss Setup und konfiguriert einen Mandanten geltende [App-Katalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) oder [Site Collection App-Katalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog), um das Webpart empfangen.]</span><span class="sxs-lookup"><span data-stu-id="8d1b9-105">You or your Office 365 Administrator must have setup and configured a tenant-wide [App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) or a [Site Collection App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)to receive the webpart.]</span></span>
- <span data-ttu-id="8d1b9-p102">Wir unterstützen nur SharePoint Online. Das Webpart wird nicht unterstützt für die Installation auf eine beliebige Version von SharePoint lokal.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-p102">We support SharePoint Online only. The web part is not support for installation on any version of SharePoint on premises.</span></span>

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a><span data-ttu-id="8d1b9-108">Hinzufügen des benutzerdefinierte Learning-Webparts zu Ihrem Mandanten</span><span class="sxs-lookup"><span data-stu-id="8d1b9-108">Add the Custom Learning webpart to your tenant</span></span> 

1. <span data-ttu-id="8d1b9-p103">Laden Sie das benutzerdefinierte Learning-Webpart, und speichern Sie sie auf Ihrem lokalen Laufwerk.  Dieser Datei lautet "ms-benutzerdefinierte-learning.sppkg".  Ändern Sie den Namen oder die Suffix der Datei nicht.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-p103">Download the Custom Learning webpart and save it to your local drive.  This file is named "ms-custom-learning.sppkg".  Do not change the name or suffix of the file.</span></span> 
2. <span data-ttu-id="8d1b9-112">Navigieren Sie zu der [Office 365-Verwaltungsportal](https://admin.microsoft.com/AdminPortal/Home#/homepage) für Ihre Mandanten</span><span class="sxs-lookup"><span data-stu-id="8d1b9-112">Navigate to the [Office 365 Admin portal](https://admin.microsoft.com/AdminPortal/Home#/homepage) for your tenant</span></span>
3. <span data-ttu-id="8d1b9-p104">Wählen Sie im linken Navigationsbereich Admin Center, SharePoint aus. Dadurch wird eine neue Registerkarte, und wählen Sie Apps In the SharePoint Admin Center, App-Katalog, Apps für SharePoint geöffnet.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-p104">From the left navigation select Admin Centers, SharePoint. This will open in a new tab. , In the SharePoint Admin Center select Apps, App Catalog, Apps for SharePoint</span></span> 
4. <span data-ttu-id="8d1b9-115">Aktivieren Sie das Webpart hochladen und wählen Sie die heruntergeladene Datei "ms-benutzerdefinierte-learning.sppkg"</span><span class="sxs-lookup"><span data-stu-id="8d1b9-115">Select upload the webpart and choose the "ms-custom-learning.sppkg" file you downloaded</span></span>
5. <span data-ttu-id="8d1b9-116">Für diese Mandanten geltende Installation das Kontrollkästchen Sie neben "Diese Lösung für alle befindet sich in der Organisation verfügbar machen."</span><span class="sxs-lookup"><span data-stu-id="8d1b9-116">For this tenant-wide installation check the box next to "Make this solution available to all sits in the organization."</span></span>  

![Bereitstellen der Lösung](media/trustapp_sm.png)


## <a name="add-the-customer-learning-webpart-to-a-sharepoint-online-page"></a><span data-ttu-id="8d1b9-118">Hinzufügen des Kunden Learning-Webparts zu einer SharePoint Online-Seite</span><span class="sxs-lookup"><span data-stu-id="8d1b9-118">Add the Customer Learning webpart to a SharePoint Online Page</span></span>

<span data-ttu-id="8d1b9-p105">Nach der Installation benutzerdefinierte Learning in Ihrem Mandanten können Sie das Webpart zu einer SharePoint-Seite hinzufügen. Wenn Sie dies tun, ist plötzlich Office 365-Schulung für Sie verfügbar.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-p105">After Custom Learning is installed in your tenant you can add the Web part to a SharePoint page. When you do, suddenly Office 365 training is available to you.</span></span> 

1. <span data-ttu-id="8d1b9-121">Fügen Sie die benutzerdefinierte Learning-Webpart in ein Layout mit voller Breite Spalten hinzu:</span><span class="sxs-lookup"><span data-stu-id="8d1b9-121">Add the Custom Learning webpart in a full width column layout:</span></span>

![SharePoint-Seitenlayout](media/clo365fullcolumnwidth.png)

2. <span data-ttu-id="8d1b9-p106">Wählen Sie im Abschnitt hinzufügen, und wählen Sie dann volle Breitenspalte, in der SharePoint-Seite.  Sehen Sie die folgende Meldung angezeigt:</span><span class="sxs-lookup"><span data-stu-id="8d1b9-p106">In the SharePoint page, select Add section and then select full width column.  You'll see the following prompt:</span></span>

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. <span data-ttu-id="8d1b9-p107">Wählen Sie Microsoft Learning.  Sie sollten nun Folgendes angezeigt:</span><span class="sxs-lookup"><span data-stu-id="8d1b9-p107">Select Microsoft Learning.  You should now see the following:</span></span> 

![Benutzerdefinierte Webpart lernen](media/clo365addwebpart.png)

 <span data-ttu-id="8d1b9-129">Sie können nun auf die Kacheln zum Untersuchen des Standardinhalts in der Projektmappe enthaltenen klicken.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-129">You can now click on the tiles to explore the default content included in the solution.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="8d1b9-130">Weitere Schritte</span><span class="sxs-lookup"><span data-stu-id="8d1b9-130">Next Steps</span></span>
- <span data-ttu-id="8d1b9-131">Verwenden Sie das [Standardkonto](webpartcontent.md) in das Webpart aus.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-131">Explore the [default content](webpartcontent.md) included in the webpart.</span></span>
- <span data-ttu-id="8d1b9-132">[Anpassen](customization.md) der Schulung Erfahrung für Ihre Organisation.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-132">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="8d1b9-133">[Bessere Akzeptanz](driveadoption.md) der Schulung Lösung ist.</span><span class="sxs-lookup"><span data-stu-id="8d1b9-133">[Drive adoption](driveadoption.md) of your training solution.</span></span>

