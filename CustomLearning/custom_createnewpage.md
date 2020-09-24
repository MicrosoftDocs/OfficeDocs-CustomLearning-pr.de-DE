---
author: pkrebs
ms.author: pkrebs
title: Erstellen von SharePoint-Seiten für Wiedergabelisten
ms.date: 02/10/2019
description: Erstellen von SharePoint-Seiten für Wiedergabelisten
ms.service: sharepoint online
ms.openlocfilehash: 99425b9be685a8090394ecb446a7c82dee24fe5d
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/23/2020
ms.locfileid: "48234507"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="62d93-103">Erstellen von SharePoint-Seiten für benutzerdefinierte Wiedergabelisten</span><span class="sxs-lookup"><span data-stu-id="62d93-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="62d93-104">Eines der einzigartigen Features von Lernpfaden ist die Möglichkeit, Wiedergabelisten zu erstellen, die aus Objekten aus Microsoft und aus von Ihnen erstellten SharePoint-Objekten zusammengesetzt werden.</span><span class="sxs-lookup"><span data-stu-id="62d93-104">One of the unique features of learning pathways is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="62d93-105">In diesem Beispiel erstellen wir eine SharePoint-Seite, bevor Sie eine Wiedergabeliste erstellen.</span><span class="sxs-lookup"><span data-stu-id="62d93-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="62d93-106">Die Möglichkeit zum Erstellen von Wiedergabelisten von SharePoint-Seiten bietet eine Vielzahl von Möglichkeiten zum Erstellen von Seiten mit den von Microsoft oder Ihrer Organisation verfügbaren Webparts.</span><span class="sxs-lookup"><span data-stu-id="62d93-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="62d93-107">Beispielsweise kann eine Wiedergabeliste eine SharePoint-Seite mit eingebetteten Videos von YouTube oder ein aus Office 365 Formularen erstelltes Formular oder einen eingebetteten Power BI-Bericht enthalten.</span><span class="sxs-lookup"><span data-stu-id="62d93-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="62d93-108">In diesem Beispiel wird gezeigt, wie Sie eine Seite mit dem embed-Webpart und dem Text-Webpart erstellen.</span><span class="sxs-lookup"><span data-stu-id="62d93-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="62d93-109">Erstellen einer SharePoint-Seite für eine benutzerdefinierte Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="62d93-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="62d93-110">Klicken Sie auf das Symbol SharePoint **Gear** , und klicken Sie dann auf **Seite hinzufügen**.</span><span class="sxs-lookup"><span data-stu-id="62d93-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="62d93-111">Klicken Sie auf der linken Seite auf **einen neuen Abschnitt hinzufügen (+)** , und klicken Sie dann auf **zwei Spalten** für das Abschnittslayout.</span><span class="sxs-lookup"><span data-stu-id="62d93-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="62d93-112">Klicken Sie in der linken Spalte auf +, und klicken Sie dann auf das Webpart **einbetten** .</span><span class="sxs-lookup"><span data-stu-id="62d93-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="62d93-113">Klicken Sie in der rechten Spalte auf +, und klicken Sie dann auf das Webpart **Text** .</span><span class="sxs-lookup"><span data-stu-id="62d93-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="62d93-114">Ihre Seite sollte wie folgt aussehen.</span><span class="sxs-lookup"><span data-stu-id="62d93-114">Your page should look like this.</span></span>

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="62d93-116">Hinzufügen eines Videos und Texts aus YouTube</span><span class="sxs-lookup"><span data-stu-id="62d93-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="62d93-117">Wechseln Sie in Ihrem Browser zu YouTube.</span><span class="sxs-lookup"><span data-stu-id="62d93-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="62d93-118">Suchen Sie in diesem Beispiel nach "Was ist Office 365 – die besten Produktivitäts-apps von Microsoft".</span><span class="sxs-lookup"><span data-stu-id="62d93-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="62d93-119">Klicken Sie auf das Video, um es wiederzugeben, halten Sie es dann an, und klicken Sie dann mit der rechten Maustaste darauf.</span><span class="sxs-lookup"><span data-stu-id="62d93-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="62d93-120">Klicken Sie auf **embed-Code kopieren**und dann zur SharePoint-Seite zurückkehren.</span><span class="sxs-lookup"><span data-stu-id="62d93-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="62d93-121">Klicken Sie im **embed** -Webpart auf **eingebetteten Code hinzufügen** , und fügen Sie dann den Code aus dem YouTube-Video hinzu.</span><span class="sxs-lookup"><span data-stu-id="62d93-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="62d93-122">Kehren Sie zur Seite YouTube zurück, und kopieren Sie den **Beschreibungs** Text für das Video.</span><span class="sxs-lookup"><span data-stu-id="62d93-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="62d93-123">Kehren Sie zur SharePoint-Seite zurück, wählen Sie das Webpart **Text** aus, und kopieren Sie dann den Text aus dem YouTube-Video.</span><span class="sxs-lookup"><span data-stu-id="62d93-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="62d93-124">Wählen Sie das Symbol " **Webpart bearbeiten** " im Titelbereich der SharePoint-Seite aus, und nennen Sie die Seite "benutzerdefinierte Wiedergabeliste".</span><span class="sxs-lookup"><span data-stu-id="62d93-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="62d93-125">Wählen Sie für **Layout**die Option **Plain**aus, und schließen Sie den Bereich Eigenschaften des **Titelbereichs** .</span><span class="sxs-lookup"><span data-stu-id="62d93-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="62d93-126">Die Seite sollte nun etwa wie folgt aussehen.</span><span class="sxs-lookup"><span data-stu-id="62d93-126">The page should now look something like the following.</span></span> 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="62d93-128">Veröffentlichen der Seite</span><span class="sxs-lookup"><span data-stu-id="62d93-128">Publish the page</span></span>

- <span data-ttu-id="62d93-129">Klicken Sie auf die Schaltfläche **veröffentlichen** .</span><span class="sxs-lookup"><span data-stu-id="62d93-129">Select the **Publish** button.</span></span> <span data-ttu-id="62d93-130">Jetzt können Sie diese SharePoint-Seite zu Ihrer benutzerdefinierten Wiedergabeliste hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="62d93-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 