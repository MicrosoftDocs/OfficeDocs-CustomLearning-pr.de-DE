---
author: pkrebs
ms.author: pkrebs
title: Erstellen von SharePoint-Seiten für Wiedergabelisten
ms.date: 02/10/2019
description: Erstellen von SharePoint-Seiten für Wiedergabelisten
ms.service: sharepoint-online
ms.openlocfilehash: 40c249fbd5b0fdaefd555f23bf20ac23240ea954
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999086"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a><span data-ttu-id="8bf14-103">Erstellen von SharePoint-Seiten für benutzerdefinierte Wiedergabelisten</span><span class="sxs-lookup"><span data-stu-id="8bf14-103">Create SharePoint pages for Custom Playlists</span></span>

<span data-ttu-id="8bf14-104">Eines der einzigartigen Features von Lernpfaden ist die Möglichkeit, Wiedergabelisten zu erstellen, die aus Ressourcen von Microsoft und aus erstellten SharePoint-Ressourcen zusammengestellt werden.</span><span class="sxs-lookup"><span data-stu-id="8bf14-104">One of the unique features of learning pathways is the ability to create playlists that are assembled from assets from Microsoft and from SharePoint assets that you create.</span></span> <span data-ttu-id="8bf14-105">In diesem Beispiel erstellen wir vor dem Erstellen einer Wiedergabeliste eine SharePoint-Seite.</span><span class="sxs-lookup"><span data-stu-id="8bf14-105">In this example, we’ll create a SharePoint page in advance of creating a playlist.</span></span> <span data-ttu-id="8bf14-106">Die Möglichkeit, Wiedergabelisten aus SharePoint-Seiten zu erstellen, bietet eine Vielzahl von Möglichkeiten zum Erstellen von Seiten mithilfe der von Microsoft oder Ihrer Organisation verfügbaren Webparts.</span><span class="sxs-lookup"><span data-stu-id="8bf14-106">The ability to build playlists from SharePoint pages offers a variety of opportunities to build pages using the Web parts available from Microsoft or your organization.</span></span> <span data-ttu-id="8bf14-107">Eine Wiedergabeliste kann z. B. eine SharePoint-Seite mit eingebetteten Videos aus YouTube oder ein aus Office 365 Forms erstelltes Formular oder einen eingebetteten Power BI-Bericht enthalten.</span><span class="sxs-lookup"><span data-stu-id="8bf14-107">For example, a playlist can include a SharePoint page with embedded videos from YouTube, or a form built from Office 365 Forms, or an embedded Power BI report.</span></span> <span data-ttu-id="8bf14-108">In diesem Beispiel wird gezeigt, wie Sie eine Seite mit dem Embed-Web part und dem Text-Web part erstellen.</span><span class="sxs-lookup"><span data-stu-id="8bf14-108">In this example, we’ll show you how to build a page with the Embed web part and the Text web part.</span></span>  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a><span data-ttu-id="8bf14-109">Erstellen einer SharePoint-Seite für eine benutzerdefinierte Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="8bf14-109">Create a SharePoint page for a custom playlist</span></span>

1. <span data-ttu-id="8bf14-110">Klicken Sie auf das Symbol SharePoint **Gear,** und klicken Sie dann **auf Seite hinzufügen.**</span><span class="sxs-lookup"><span data-stu-id="8bf14-110">Click the SharePoint **Gear** icon, and then click **Add a page**.</span></span>
2. <span data-ttu-id="8bf14-111">Klicken Sie auf der linken Seite der Seite auf Neuen Abschnitt **hinzufügen (+),** und klicken Sie dann auf **Zwei** Spalten für das Abschnittslayout.</span><span class="sxs-lookup"><span data-stu-id="8bf14-111">Click **Add a new section (+)** on the left-hand side of the page, and then click **Two Columns** for the section layout.</span></span>
3. <span data-ttu-id="8bf14-112">Klicken Sie in der linken Spalte auf + , und klicken Sie dann auf web part **einbetten.**</span><span class="sxs-lookup"><span data-stu-id="8bf14-112">In the left column, click + , and then click the **Embed** web part.</span></span> 
4. <span data-ttu-id="8bf14-113">Klicken Sie in der rechten Spalte auf  +, und klicken Sie dann auf das Textwebteil.</span><span class="sxs-lookup"><span data-stu-id="8bf14-113">In the right column, click +, and then click the **Text** web part.</span></span> <span data-ttu-id="8bf14-114">Ihre Seite sollte wie dies aussehen.</span><span class="sxs-lookup"><span data-stu-id="8bf14-114">Your page should look like this.</span></span>

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a><span data-ttu-id="8bf14-116">Hinzufügen eines Videos und Texts aus YouTube</span><span class="sxs-lookup"><span data-stu-id="8bf14-116">Add a video and text from YouTube</span></span>

1. <span data-ttu-id="8bf14-117">Wechseln Sie in Ihrem Browser zu YouTube.</span><span class="sxs-lookup"><span data-stu-id="8bf14-117">In your browser, go to YouTube.</span></span> <span data-ttu-id="8bf14-118">Suchen Sie in diesem Beispiel nach "Was ist Office 365 – Die besten Produktivitäts-Apps von Microsoft".</span><span class="sxs-lookup"><span data-stu-id="8bf14-118">For this example, search for “What is Office 365 – Microsoft’s best productivity apps”.</span></span>
2. <span data-ttu-id="8bf14-119">Klicken Sie auf das Video, um es wieder zu spielen, halten Sie es an, und klicken Sie dann mit der rechten Maustaste darauf.</span><span class="sxs-lookup"><span data-stu-id="8bf14-119">Click the video to play it, then pause it, then right-click on it.</span></span> 
3. <span data-ttu-id="8bf14-120">Klicken **Sie auf Einbettungscode** kopieren, und kehren Sie dann zur SharePoint-Seite zurück.</span><span class="sxs-lookup"><span data-stu-id="8bf14-120">Click **Copy embed code**, then return to the SharePoint page.</span></span> 
4. <span data-ttu-id="8bf14-121">Klicken **Sie im** **Web** part Embed auf Einbettungscode hinzufügen, und fügen Sie dann den Code aus dem YouTube-Video hinzu.</span><span class="sxs-lookup"><span data-stu-id="8bf14-121">Click **Add embed code** in the **Embed** web part, and then add the code from the YouTube video.</span></span>
5. <span data-ttu-id="8bf14-122">Kehren Sie zur YouTube-Seite zurück, und kopieren Sie **den Beschreibungstext** für das Video.</span><span class="sxs-lookup"><span data-stu-id="8bf14-122">Return to the YouTube page and copy the **Description** text for the video.</span></span> 
6. <span data-ttu-id="8bf14-123">Kehren Sie zur Seite SharePoint zurück, wählen Sie das **Textwebteil** aus, und kopieren Sie dann den Text aus dem YouTube-Video.</span><span class="sxs-lookup"><span data-stu-id="8bf14-123">Return to the SharePoint page, select the **Text** web part, then copy the text from the YouTube video.</span></span>
7. <span data-ttu-id="8bf14-124">Wählen Sie **das Symbol Webteil** bearbeiten im Bereich Titel der SharePoint-Seite aus, und nennen Sie dann die Seite "Benutzerdefinierte Wiedergabelisteneinführung".</span><span class="sxs-lookup"><span data-stu-id="8bf14-124">Select the **Edit web part** icon  in the Title area of the SharePoint page, and then name the page “Custom Playlist Introduction”.</span></span> 
8. <span data-ttu-id="8bf14-125">Wählen **Sie unter Layout** die Option **Nur** aus, und schließen Sie dann den **Eigenschaftenbereich Titelbereich.**</span><span class="sxs-lookup"><span data-stu-id="8bf14-125">For **Layout**, select **Plain**, then close **Title Region** properties pane.</span></span> <span data-ttu-id="8bf14-126">Die Seite sollte nun etwa wie folgt aussehen.</span><span class="sxs-lookup"><span data-stu-id="8bf14-126">The page should now look something like the following.</span></span> 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a><span data-ttu-id="8bf14-128">Veröffentlichen der Seite</span><span class="sxs-lookup"><span data-stu-id="8bf14-128">Publish the page</span></span>

- <span data-ttu-id="8bf14-129">Wählen Sie die **Schaltfläche Veröffentlichen** aus.</span><span class="sxs-lookup"><span data-stu-id="8bf14-129">Select the **Publish** button.</span></span> <span data-ttu-id="8bf14-130">Jetzt können Sie diese SharePoint-Seite ihrer benutzerdefinierten Wiedergabeliste hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="8bf14-130">Now you're ready to add this SharePoint page to your custom playlist.</span></span> 