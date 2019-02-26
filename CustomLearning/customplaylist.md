---
author: karuanag
ms.author: karuanag
title: Anpassen und Freigeben von Wiedergabelisten
ms.date: 02/10/2019
description: Erstellen benutzerdefinierter Wiedergabelisten aus vorhandenen Inhalten oder neuen SharePoint-Seiten
ms.openlocfilehash: d330b6e401c9020eb68877bc8a132350811a2f31
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989726"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="c3026-103">Anpassen und Freigeben von Wiedergabelisten</span><span class="sxs-lookup"><span data-stu-id="c3026-103">Customize and Share Playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="c3026-104">Erstellen einer Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="c3026-104">Create a Playlist</span></span>

<span data-ttu-id="c3026-p101">Eine Wiedergabeliste ist die Einhaltung von "Assets". Ein "Asset" ist eine SharePoint-Seite oder ein vorhandenes Element von Microsoft-Schulungsinhalten. Wenn Sie eine Wiedergabeliste erstellen, wählen Sie Objekte aus, die gemeinsam einen Lernpfad für Ihren Benutzer erstellen.</span><span class="sxs-lookup"><span data-stu-id="c3026-p101">A playlist is a compliation of "assets". An "asset" is a SharePoint page or existing item of Microsoft training content. When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="c3026-p102">Der Vorteil beim Hinzufügen von SharePoint-Seiten besteht darin, dass Sie SharePoint-Seiten mit YouTube-Videos oder-Videos erstellen können, die in Ihrer Organisation gehostet werden. Sie können auch Seiten mit Formularen oder anderen Office 365-Inhalten erstellen.</span><span class="sxs-lookup"><span data-stu-id="c3026-p102">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization. You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="c3026-110">Schritt 1: Erstellen einer SharePoint-Seite für Ihre Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="c3026-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="c3026-p103">In diesem Beispiel erstellen wir zunächst eine SharePoint-Seite, die der Wiedergabeliste hinzugefügt werden soll. Wir erstellen eine Seite mit einem YouTube-Video-Webpart und einem Text WebPart.  Bei diesen Anweisungen wird davon ausgegangen, dass Sie den SharePoint Online-Dienst verwenden.</span><span class="sxs-lookup"><span data-stu-id="c3026-p103">In this example, we’ll first create a SharePoint page to add to the playlist. We’ll create a page with a YouTube video web part and Text web part.  These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="c3026-114">Erstellen einer neuen Seite</span><span class="sxs-lookup"><span data-stu-id="c3026-114">Create a new page</span></span>
1.  <span data-ttu-id="c3026-115">Wählen Sie das Menü Einstellungen > Site Contents > Site Pages > New > Site Page aus.</span><span class="sxs-lookup"><span data-stu-id="c3026-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="c3026-116">Geben Sie im Bereich Titel den Befehl Teams verwenden ein.</span><span class="sxs-lookup"><span data-stu-id="c3026-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="c3026-117">Wählen Sie den Abschnitt neuen hinzufügen aus, und wählen Sie dann zwei Spalten aus.</span><span class="sxs-lookup"><span data-stu-id="c3026-117">Select the Add a new section, and then select Two Columns.</span></span>

![zwei Spalten hinzufügen](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="c3026-119">Klicken Sie im linken Feld auf neues Webpart hinzufügen, und wählen Sie dann einBetten aus.</span><span class="sxs-lookup"><span data-stu-id="c3026-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="c3026-120">Wechseln Sie in einem Webbrowser zu dieser URL https://youtu.be/wYrRCRphrp0 , und rufen Sie den embed-Code für das Video ab.</span><span class="sxs-lookup"><span data-stu-id="c3026-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="c3026-121">Wählen Sie im SharePoint-Webpart embed-Code hinzufügen aus, und fügen Sie ihn dann in das Feld embed ein.</span><span class="sxs-lookup"><span data-stu-id="c3026-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="c3026-122">Klicken Sie im rechten Feld auf neues Webpart hinzufügen, und wählen Sie dann Text aus.</span><span class="sxs-lookup"><span data-stu-id="c3026-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="c3026-p104">Wechseln Sie in einem Webbrowser zu dieser URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b , und kopieren Sie die try it! Anweisungen auf der Seite und fügen Sie Sie in das Text Webpart ein. Ihre Seite sollte wie folgt aussehen.</span><span class="sxs-lookup"><span data-stu-id="c3026-p104">In a Web browser, go to this URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it! Instructions from the page and paste them into the Text Web part. Your page should look like the following.</span></span> 

![Seite einBetten](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="c3026-127">Klicken Sie auf **veröffentlichen**, und kopieren Sie dann die URL der Seite, und fügen Sie Sie in Notepad ein.</span><span class="sxs-lookup"><span data-stu-id="c3026-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="c3026-128">Schritt 2: Erstellen der Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="c3026-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="c3026-p105">Navigieren Sie zur **benutzerdefinierten Learning Administration** -Seite in der Websiteumgebung. ![custom_admin. png](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="c3026-p105">Navigate to the **Custom Learning Administration** page in your site experience. ![custom_admin.png](media/custom_admin.png)</span></span>
1. <span data-ttu-id="c3026-131">Stellen Sie sicher, dass **Kategorie** ausgewählt ist.</span><span class="sxs-lookup"><span data-stu-id="c3026-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="c3026-132">Klicken Sie auf die Kategorie, in der die neue Wiedergabeliste angezeigt werden soll.</span><span class="sxs-lookup"><span data-stu-id="c3026-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="c3026-133">Klicken Sie neben dem Namen der Kategorie auf das Pluszeichen ![custom_addplay. png.](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="c3026-133">Next to the category name, click on the plus symbol ![custom_addplay.png](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="c3026-p106">Geben Sie die Werte wie im folgenden Beispiel ein, und wählen Sie **Erstellen**aus. ![custom_details. png](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="c3026-p106">Fill in the values as shown in the example below and select **Create**. ![custom_details.png](media/custom_details.png)</span></span>
- <span data-ttu-id="c3026-136">**Title** – Anzeigename der Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="c3026-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="c3026-137">**Beschreibung** – Informationen zu den erlernten</span><span class="sxs-lookup"><span data-stu-id="c3026-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="c3026-138">**Kategorie** -vorab ausgewählt basierend auf der anfänglichen Auswahl</span><span class="sxs-lookup"><span data-stu-id="c3026-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="c3026-139">**Unterkategorie** – ausgewählt basierend auf Ihrer anfänglichen Auswahl</span><span class="sxs-lookup"><span data-stu-id="c3026-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="c3026-140">**Technologie** – Auswahl nach Bedarf</span><span class="sxs-lookup"><span data-stu-id="c3026-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="c3026-141">**Stufe** – Anfänger, Intermidate oder erweitert</span><span class="sxs-lookup"><span data-stu-id="c3026-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="c3026-142">Ziel **Gruppe** – auf diese Weise können Sie Inhalte basierend auf einer vordefinierten Liste von Rollen, die von Microsoft bereitgestellt werden, ausrichten.</span><span class="sxs-lookup"><span data-stu-id="c3026-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="c3026-143">Klicken Sie auf **Details speichern**</span><span class="sxs-lookup"><span data-stu-id="c3026-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="c3026-p107">Sie können das Symbolbild für Ihre Wiedergabeliste anpassen.  Klicken Sie auf das Bildsymbol, und fügen Sie eine URL eines zuvor hochgeladenen Bilds ein.  Stellen Sie sicher, dass sich das Bild in der benutzerdefinierten Learning-Websitesammlung oder an einem anderen Speicherort befindet, auf den alle Benutzer Zugriff auf die Datei haben.</span><span class="sxs-lookup"><span data-stu-id="c3026-p107">You can customize the icon image for your playlist.  Click the image icon and insert an URL of a previously uploaded image.  Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="c3026-147">![custom_image. png](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="c3026-147">![custom_image.png](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="c3026-148">Schritt 3: Hinzufügen von Objekten zur Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="c3026-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="c3026-149">In diesem Schritt fügen Sie vorhandene Objekte aus Microsoft und die von Ihnen erstellte SharePoint-Seite der Wiedergabeliste hinzu.</span><span class="sxs-lookup"><span data-stu-id="c3026-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="c3026-150">Nachdem Sie die Details für Ihre Wiedergabeliste gespeichert haben, können Sie die Suche nach vorhandenen Objekten verwenden.</span><span class="sxs-lookup"><span data-stu-id="c3026-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="c3026-p108">**Geben Sie in einen beliebigen Suchbegriff** ein, um eine Liste der vordefinierten Objekte anzuzeigen, die von anderen Wiedergabelisten zur Verfügung stehen. **Klicken Sie auf den Namen** eines Objekts, um es in die neue Wiedergabeliste einzufügen. ![custom_slist. png](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="c3026-p108">**Enter in any search term** to see a list of predefined assets that are available from other playlists. **Click on the name** of an asset to include it in your new playlist. ![custom_slist.png](media/custom_slist.png)</span></span>

<span data-ttu-id="c3026-154">Sie können auch die zuvor erstellte SharePoint-Seite hinzufügen oder eine von Grund auf neu erstellen.</span><span class="sxs-lookup"><span data-stu-id="c3026-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="c3026-155">Klicken Sie im Dialogfeld "Wiedergabelisten Objekte" auf die Option " **Neues Element** ".</span><span class="sxs-lookup"><span data-stu-id="c3026-155">Click on the **New Asset** option in the Playlist Assets dialog</span></span>
1. <span data-ttu-id="c3026-p109">Geben Sie Ihrem Asset einen **Titel**. Nach der Eingabe werden zusätzliche Optionen custom_newpage ![. png angezeigt.](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="c3026-p109">Give your asset a **Title**. Once entered, additional options will display ![custom_newpage.png](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="c3026-158">Sie können jetzt eine neue Objekt Seite in SharePoint Online erstellen oder die URL einer vorhandenen Seite eingeben, um Sie Ihrer benutzerdefinierten Wiedergabeliste hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="c3026-158">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="c3026-159">**Kategorien**-, **Unterkategorie** -und **Technologie** Felder werden basierend auf Ihrer vorherigen Auswahl für diese Wiedergabeliste vorab aufgefüllt.</span><span class="sxs-lookup"><span data-stu-id="c3026-159">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="c3026-160">Treffen Sie die richtige Auswahl für Ebene und Zielgruppe für dieses einzelne Objekt.</span><span class="sxs-lookup"><span data-stu-id="c3026-160">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="c3026-161">Klicken Sie auf **Ressource speichern** , um Sie der benutzerdefinierten Wiedergabeliste hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="c3026-161">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="c3026-162">Wiederholen Sie diese Schritte, indem Sie einzelne Seiten durchsuchen oder hinzufügen, bis die Wiedergabeliste abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="c3026-162">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="c3026-163">Klicken Sie auf **Wiedergabeliste** zum Speichern Beenden</span><span class="sxs-lookup"><span data-stu-id="c3026-163">Click **Close Playlist** to save</span></span>

<span data-ttu-id="c3026-164">Ihre Wiedergabeliste mit diesem Inhalt ist jetzt verfügbar, wenn Sie das benutzerdefinierte Lern Webpart installiert/eingebettet haben.</span><span class="sxs-lookup"><span data-stu-id="c3026-164">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="c3026-165">Wenn Sie einen Fehler gemacht haben, nachdem Sie die Wiedergabeliste geschlossen haben, können Sie Sie aus der Kategorie löschen, indem Sie auf das X neben dem Namen der Wiedergabeliste klicken.</span><span class="sxs-lookup"><span data-stu-id="c3026-165">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="c3026-166">Zu berücksichtigende Aspekte</span><span class="sxs-lookup"><span data-stu-id="c3026-166">Things to Think About</span></span>

<span data-ttu-id="c3026-p110">Benutzerdefinierte Wiedergabelisten können verwendet werden, um Ihre Endbenutzer bei einer Vielzahl von Aufgaben zu unterstützen.  Haben Sie ein Formular für die Ausfallszeit?  Ein Formular zum Anfordern von Hardwaregeräten?  Vorhandene Trainings Objekte können in die Umgebung einprogrammiert werden.</span><span class="sxs-lookup"><span data-stu-id="c3026-p110">Custom playlists can be used to assist your end users in a variety of tasks.  Do you have a time off request form?  A form to request hardware equipment?  Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="c3026-171">Freigeben von Wiedergabelisten</span><span class="sxs-lookup"><span data-stu-id="c3026-171">Share Playlists</span></span>

1. <span data-ttu-id="c3026-172">Navigieren Sie zu einer beliebigen Wiedergabeliste innerhalb der Webpart-oder Websiteumgebung.</span><span class="sxs-lookup"><span data-stu-id="c3026-172">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="c3026-173">In der oberen linken Ecke werden drei Symbole angezeigt.</span><span class="sxs-lookup"><span data-stu-id="c3026-173">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="c3026-174">Klicken Sie auf das Symbol, das einen Link darstellt.</span><span class="sxs-lookup"><span data-stu-id="c3026-174">Click on the icon representing a link</span></span>
1. <span data-ttu-id="c3026-175">Kopieren der URL in die Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="c3026-175">Copy the URL to the playlist</span></span>

<span data-ttu-id="c3026-176">![share. png](media/share.png) diese URL kann jetzt in Ihre Websitenavigation eingefügt oder in anderer Kommunikation verwendet werden, um Ihre Mitarbeiter direkt zu dieser Wiedergabeliste zu übertragen.</span><span class="sxs-lookup"><span data-stu-id="c3026-176">![share.png](media/share.png) This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoptiondriveadoptionmd"></a><span data-ttu-id="c3026-177">Nächste Schritte- [Einführung](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="c3026-177">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
