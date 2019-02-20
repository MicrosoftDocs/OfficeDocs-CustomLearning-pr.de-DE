---
author: pkrebs
ms.author: pkrebs
title: Erstellen von SharePoint-Seiten für Wiedergabelisten
ms.date: 02/10/2019
description: Erstellen von SharePoint-Seiten für Wiedergabelisten
ms.openlocfilehash: c2de66a0746260e8f6539656ad70052b209c54ba
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/19/2019
ms.locfileid: "30103690"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="ea556-103">Erstellen von SharePoint-Seiten für benutzerdefinierte Wiedergabelisten</span><span class="sxs-lookup"><span data-stu-id="ea556-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="ea556-p101">Eine der einzigartigen Features von benutzerdefiniertem lernen ist die Möglichkeit, Wiedergabelisten zu erstellen, die aus Objekten aus Microsoft und aus von Ihnen erstellten SharePoint-Objekten zusammengestellt werden. In diesem Beispiel erstellen wir eine SharePoint-Seite vor dem Erstellen einer Wiedergabeliste. Die Möglichkeit, Wiedergabelisten von SharePoint-Seiten zu erstellen, bietet eine Vielzahl von Möglichkeiten zum Erstellen von Seiten mithilfe der Webparts, die von Microsoft oder Ihrer Organisation zur Verfügung stehen. Eine Wiedergabeliste kann beispielsweise eine SharePoint-Seite mit eingebetteten Videos von YouTube oder ein aus Office 365-Formularen erstelltes Formular oder einen eingebetteten Power BI-Bericht aufweisen. In diesem Beispiel wird gezeigt, wie Sie eine Seite mit dem Webpart "embed" und dem Webpart "Text" erstellen.</span><span class="sxs-lookup"><span data-stu-id="ea556-p101">One of the unique features of Custom Learning is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create. In this example, we’ll create a SharePoint page in advance of creating a playlist. The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization. For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report. In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="ea556-109">Erstellen einer SharePoint-Seite für eine benutzerdefinierte Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="ea556-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="ea556-110">Klicken Sie auf das SharePoint **Gear** -Symbol, und klicken Sie dann auf **Seite hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="ea556-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="ea556-111">Klicken Sie Links auf der Seite auf **neuen Abschnitt hinzufügen (+)** , und klicken Sie dann auf **zwei Spalten** für das Abschnittslayout.</span><span class="sxs-lookup"><span data-stu-id="ea556-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="ea556-112">Klicken Sie in der linken Spalte auf +, und klicken Sie dann auf das Webpart **embed** .</span><span class="sxs-lookup"><span data-stu-id="ea556-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="ea556-p102">Klicken Sie in der rechten Spalte auf +, und klicken Sie dann auf das Webpart **Text** . Ihre Seite sollte wie folgt aussehen.</span><span class="sxs-lookup"><span data-stu-id="ea556-p102">In the right column, click +, and then click the **Text** web part. Your page should look like this.</span></span>

![CG-pagenewstart. png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="ea556-116">Hinzufügen eines Videos und Texts von YouTube</span><span class="sxs-lookup"><span data-stu-id="ea556-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="ea556-p103">Wechseln Sie in Ihrem Browser zu YouTube. Suchen Sie in diesem Beispiel nach "Was ist Office 365 – die besten Produktivitäts-apps von Microsoft".</span><span class="sxs-lookup"><span data-stu-id="ea556-p103">In your browser, go to YouTube. For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="ea556-119">Klicken Sie auf das Video, um es wiederzugeben, und klicken Sie dann mit der rechten Maustaste darauf.</span><span class="sxs-lookup"><span data-stu-id="ea556-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="ea556-120">Klicken Sie auf **embed-Code kopieren**und dann zur SharePoint-Seite zurückkehren.</span><span class="sxs-lookup"><span data-stu-id="ea556-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="ea556-121">Klicken Sie im **embed** -Webpart auf **embed-Code hinzufügen** , und fügen Sie dann den Code aus dem YouTube-Video hinzu.</span><span class="sxs-lookup"><span data-stu-id="ea556-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="ea556-122">Kehren Sie zur YouTube-Seite zurück \*\*\*\* , und kopieren Sie den Beschreibungstext für das Video.</span><span class="sxs-lookup"><span data-stu-id="ea556-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="ea556-123">Kehren Sie zur Seite SharePoint zurück, wählen Sie das Webpart **Text** aus, und kopieren Sie dann den Text aus dem YouTube-Video.</span><span class="sxs-lookup"><span data-stu-id="ea556-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="ea556-124">Wählen Sie das Symbol **Webpart bearbeiten** im titelBereich der SharePoint-Seite aus, und nennen Sie dann die Seite "benutzerdefinierte Playlist-Einführung".</span><span class="sxs-lookup"><span data-stu-id="ea556-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="ea556-p104">Wählen Sie unter **Layout**die Option **Plain**aus, und schließen Sie dann den Bereich **Title Region** Properties. Die Seite sollte jetzt ungefähr wie folgt aussehen.</span><span class="sxs-lookup"><span data-stu-id="ea556-p104">For **Layout**, select **Plain**, then close **Title Region** properties pane. The page should now look something like the following.</span></span> 

![CG-pagenewfinish. png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="ea556-128">Seite veröffentlichen</span><span class="sxs-lookup"><span data-stu-id="ea556-128">Publish the page</span></span>

- <span data-ttu-id="ea556-p105">Klicken Sie auf die Schaltfläche **veröffentlichen** . Jetzt können Sie diese SharePoint-Seite Ihrer benutzerdefinierten Wiedergabeliste hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="ea556-p105">Select the **Publish** button. Now you're ready to add this SharePoint page to your custom playlist.</span></span> 