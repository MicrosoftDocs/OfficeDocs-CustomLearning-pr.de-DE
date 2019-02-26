---
author: karuanag
ms.author: karuanag
title: Installieren der benutzerdefinierten Learning Solution-Webpart
ms.date: 02/10/2019
description: Installationsanweisungen für die benutzerdefinierte Lernlösung Webpart
ms.openlocfilehash: 53229e5b1b8175b06d888091963d1a9f2f0bd361
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989686"
---
# <a name="installing-the-custom-learning-solution-webpart"></a><span data-ttu-id="d9365-103">Installieren der benutzerdefinierten Learning Solution-Webpart</span><span class="sxs-lookup"><span data-stu-id="d9365-103">Installing the Custom Learning Solution Webpart</span></span>

## <a name="prerequisites-for-a-tenant-wide-installation"></a><span data-ttu-id="d9365-104">VoraussetZungen für eine Mandantenweite Installation</span><span class="sxs-lookup"><span data-stu-id="d9365-104">Prerequisites for a tenant-wide installation</span></span>

- <span data-ttu-id="d9365-p101">Um das benutzerdefinierte Lern Webpart für Ihren gesamten Mandanten zu installieren, benötigen Sie Office 365-Administratorberechtigungen.  Wenn Sie nicht über diese Berechtigungen verfügen, können Sie entweder mit Ihrem Office 365-Administrator zusammenarbeiten oder das Webpart für eine einzelne Websitesammlung installieren.</span><span class="sxs-lookup"><span data-stu-id="d9365-p101">To install the Custom Learning webpart for your entire tenant you will need to have Office 365 Administrative permissions.  If you do not have these permissions you can either work with your Office 365 Administrator or install the webpart for an individual site collection.</span></span>
- <span data-ttu-id="d9365-107">Sie oder Ihr Office 365-Administrator müssen einen Mandanten weiten [App-Katalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) oder einen [Website Sammlungs-App-Katalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)einrichten und konfigurieren, um den Webpart zu empfangen.]</span><span class="sxs-lookup"><span data-stu-id="d9365-107">You or your Office 365 Administrator must have setup and configured a tenant-wide [App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) or a [Site Collection App Catalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)to receive the webpart.]</span></span>
- <span data-ttu-id="d9365-p102">Wir unterstützen nur SharePoint Online. Das Webpart ist nicht für die Installation in einer beliebigen Version von SharePoint unterstützt.</span><span class="sxs-lookup"><span data-stu-id="d9365-p102">We support SharePoint Online only. The web part is not support for installation on any version of SharePoint on premises.</span></span>

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a><span data-ttu-id="d9365-110">Hinzufügen des benutzerdefinierten Learning-Webpart zu Ihrem Mandanten</span><span class="sxs-lookup"><span data-stu-id="d9365-110">Add the Custom Learning webpart to your tenant</span></span> 

1. <span data-ttu-id="d9365-p103">Laden Sie das benutzerdefinierte Lern Webpart herunter, und speichern Sie es auf Ihrem lokalen Laufwerk.  Diese Datei heißt "MS-Custom-Learning. sppkg".  Ändern Sie nicht den Namen oder das Suffix der Datei.</span><span class="sxs-lookup"><span data-stu-id="d9365-p103">Download the Custom Learning webpart and save it to your local drive.  This file is named "ms-custom-learning.sppkg".  Do not change the name or suffix of the file.</span></span> 
2. <span data-ttu-id="d9365-114">Navigieren Sie zum [Office 365-Verwaltungsportal](https://admin.microsoft.com/AdminPortal/Home#/homepage) für Ihren Mandanten.</span><span class="sxs-lookup"><span data-stu-id="d9365-114">Navigate to the [Office 365 Admin portal](https://admin.microsoft.com/AdminPortal/Home#/homepage) for your tenant</span></span>
3. <span data-ttu-id="d9365-p104">Wählen Sie im linken Navigationsbereich Admin Center, SharePoint aus. Sie wird in einer neuen Registerkarte geöffnet. Wählen Sie im SharePoint Admin Center apps, App-Katalog, Apps für SharePoint</span><span class="sxs-lookup"><span data-stu-id="d9365-p104">From the left navigation select Admin Centers, SharePoint. This will open in a new tab. , In the SharePoint Admin Center select Apps, App Catalog, Apps for SharePoint</span></span> 
4. <span data-ttu-id="d9365-117">Wählen Sie Webpart Hochladen aus, und wählen Sie die Datei "MS-Custom-Learning. sppkg" aus, die Sie heruntergeladen haben.</span><span class="sxs-lookup"><span data-stu-id="d9365-117">Select upload the webpart and choose the "ms-custom-learning.sppkg" file you downloaded</span></span>
5. <span data-ttu-id="d9365-118">Bei dieser Mandanten weiten Installation aktivieren Sie das Kontrollkästchen neben "Diese Lösung für alle verfügbar machen in der Organisation".</span><span class="sxs-lookup"><span data-stu-id="d9365-118">For this tenant-wide installation check the box next to "Make this solution available to all sits in the organization."</span></span>  
 
> [!NOTE]
> <span data-ttu-id="d9365-p105">Sobald das Webpart installiert ist, finden Sie es in Ihrem Webpart-Katalog in SharePoint Online.  **In der Galerie heißt das Webpart "Microsoft Learning"** .</span><span class="sxs-lookup"><span data-stu-id="d9365-p105">Once the webpart is installed you will find it in your webpart gallery in SharePoint Online.  **In the gallery the webpart is named "Microsoft Learning"**</span></span>

![Bereitstelleneiner Lösung](media/trustapp_sm.png)


## <a name="add-the-microsoft-learning-webpart-to-a-sharepoint-online-page"></a><span data-ttu-id="d9365-122">Hinzufügen des Microsoft Learning-Webpart zu einer SharePoint Online-Seite</span><span class="sxs-lookup"><span data-stu-id="d9365-122">Add the Microsoft Learning webpart to a SharePoint Online Page</span></span>

<span data-ttu-id="d9365-p106">Nachdem benutzerdefiniertes lernen in Ihrem Mandanten installiert wurde, können Sie das Webpart einer SharePoint-Seite hinzufügen. Wenn Sie Office 365 und Windows 10 trainieren, steht Ihre Website zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="d9365-p106">After Custom Learning is installed in your tenant you can add the Web part to a SharePoint page. When you do Office 365 and Windows 10 training is available to your site.</span></span>

1. <span data-ttu-id="d9365-125">Hinzufügen des benutzerdefinierten Learning-Webpart in einem Spaltenlayout mit voller Breite:</span><span class="sxs-lookup"><span data-stu-id="d9365-125">Add the Custom Learning webpart in a full width column layout:</span></span>

![SharePoint-Seiten Layout](media/clo365fullcolumnwidth.png)

2. <span data-ttu-id="d9365-p107">Wählen Sie auf der Seite SharePoint die Option Abschnitt hinzufügen aus, und wählen Sie dann Spalte vollständiger Breite aus.  Die folgende Meldung wird angezeigt:</span><span class="sxs-lookup"><span data-stu-id="d9365-p107">In the SharePoint page, select Add section and then select full width column.  You'll see the following prompt:</span></span>

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. <span data-ttu-id="d9365-p108">Wählen Sie Microsoft Learning aus.  Es sollte jetzt Folgendes angezeigt werden:</span><span class="sxs-lookup"><span data-stu-id="d9365-p108">Select Microsoft Learning.  You should now see the following:</span></span> 

![Benutzerdefiniertes Learning-Webpart](media/clo365addwebpart.png)

 <span data-ttu-id="d9365-133">Sie können nun auf die Kacheln klicken, um die in der Lösung enthaltenen Standardinhalte zu erkunden.</span><span class="sxs-lookup"><span data-stu-id="d9365-133">You can now click on the tiles to explore the default content included in the solution.</span></span>  

### <a name="next-steps"></a><span data-ttu-id="d9365-134">Weitere Schritte</span><span class="sxs-lookup"><span data-stu-id="d9365-134">Next Steps</span></span>
- <span data-ttu-id="d9365-135">Erkunden Sie die im Webpart enthaltenen [Standardinhalte](webpartcontent.md) .</span><span class="sxs-lookup"><span data-stu-id="d9365-135">Explore the [default content](webpartcontent.md) included in the webpart.</span></span>
- <span data-ttu-id="d9365-136">[Passen](customization.md) Sie die Schulungsumgebung für Ihre Organisation an.</span><span class="sxs-lookup"><span data-stu-id="d9365-136">[Customize](customization.md) the training experience for your organization.</span></span>
- <span data-ttu-id="d9365-137">Führen Sie die [Einführung](driveadoption.md) ihrer Schulungslösung aus.</span><span class="sxs-lookup"><span data-stu-id="d9365-137">[Drive adoption](driveadoption.md) of your training solution.</span></span>

