---
author: karuanag
ms.author: karuanag
title: Anpassen und Freigeben von Wiedergabelisten
ms.date: 02/10/2019
description: Erstellen benutzerdefinierter Wiedergabelisten aus vorhandenen Inhalten oder neuen SharePoint-Seiten
ms.service: sharepoint online
ms.openlocfilehash: 6258668b417ba496c7ac75e36ce2bc1f1dae27a5
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233807"
---
# <a name="customize-and-share-playlists"></a><span data-ttu-id="f01b2-103">Anpassen und Freigeben von Wiedergabelisten</span><span class="sxs-lookup"><span data-stu-id="f01b2-103">Customize and Share Playlists</span></span>

## <a name="create-a-playlist"></a><span data-ttu-id="f01b2-104">Erstellen einer Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="f01b2-104">Create a Playlist</span></span>

<span data-ttu-id="f01b2-105">Eine Wiedergabeliste entspricht "Assets".</span><span class="sxs-lookup"><span data-stu-id="f01b2-105">A playlist is a compliation of "assets".</span></span> <span data-ttu-id="f01b2-106">Ein "Asset" ist eine SharePoint-Seite oder ein vorhandenes Element von Microsoft-Schulungsinhalten.</span><span class="sxs-lookup"><span data-stu-id="f01b2-106">An "asset" is a SharePoint page or existing item of Microsoft training content.</span></span> <span data-ttu-id="f01b2-107">Wenn Sie eine Wiedergabeliste erstellen, wählen Sie Objekte aus, die zusammen gehen, um einen Lernpfad für Ihren Benutzer zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="f01b2-107">When you create a playlist you select assets that go together to create a learning path for your user.</span></span>  

<span data-ttu-id="f01b2-108">Der Vorteil des Hinzufügens von SharePoint-Seiten ist, dass Sie SharePoint-Seiten mit einem YouTube-Videos oder Videos in Ihrer Organisation gehostet erstellen können.</span><span class="sxs-lookup"><span data-stu-id="f01b2-108">The benefit of adding SharePoint pages is that you can create SharePoint pages with a YouTube videos or videos hosted in your organization.</span></span> <span data-ttu-id="f01b2-109">Sie können auch Seiten mit Formularen oder anderen Office 365 Inhalten erstellen.</span><span class="sxs-lookup"><span data-stu-id="f01b2-109">You can also create pages with Forms or other Office 365 content.</span></span>  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a><span data-ttu-id="f01b2-110">Schritt 1: Erstellen einer SharePoint-Seite für Ihre Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="f01b2-110">Step 1: Create a SharePoint page for your playlist</span></span>
<span data-ttu-id="f01b2-111">In diesem Beispiel erstellen wir zunächst eine SharePoint-Seite, die der Wiedergabeliste hinzugefügt werden soll.</span><span class="sxs-lookup"><span data-stu-id="f01b2-111">In this example, we’ll first create a SharePoint page to add to the playlist.</span></span> <span data-ttu-id="f01b2-112">Wir erstellen eine Seite mit einem YouTube-Video-Webpart und einem Text-WebPart.</span><span class="sxs-lookup"><span data-stu-id="f01b2-112">We’ll create a page with a YouTube video web part and Text web part.</span></span>  <span data-ttu-id="f01b2-113">Bei diesen Anweisungen wird davon ausgegangen, dass Sie den SharePoint Online Dienst verwenden.</span><span class="sxs-lookup"><span data-stu-id="f01b2-113">These instructions assume you are using the SharePoint Online service.</span></span> 

#### <a name="create-a-new-page"></a><span data-ttu-id="f01b2-114">Eine neue Seite erstellen</span><span class="sxs-lookup"><span data-stu-id="f01b2-114">Create a new page</span></span>
1.  <span data-ttu-id="f01b2-115">Wählen Sie das Menü Einstellungen > Websiteinhalte > Website Seiten > Seite neue > Site aus.</span><span class="sxs-lookup"><span data-stu-id="f01b2-115">Select the Settings menu > Site Contents > Site Pages > New > Site Page.</span></span>
2.  <span data-ttu-id="f01b2-116">Geben Sie im Bereich Titel den Befehl Teams verwenden ein.</span><span class="sxs-lookup"><span data-stu-id="f01b2-116">In the title area, type Use the Teams command box</span></span>
3.  <span data-ttu-id="f01b2-117">Wählen Sie den Abschnitt neuen Abschnitt hinzufügen aus, und wählen Sie dann zwei Spalten aus.</span><span class="sxs-lookup"><span data-stu-id="f01b2-117">Select the Add a new section, and then select Two Columns.</span></span>

![zweispaltige hinzufügen](media/clo365addtwocolumn.png)

4.  <span data-ttu-id="f01b2-119">Wählen Sie im linken Feld Neues Webpart hinzufügen aus, und wählen Sie dann einbetten aus.</span><span class="sxs-lookup"><span data-stu-id="f01b2-119">In the left-hand box, select Add a new web part, and then select Embed.</span></span> 
5.  <span data-ttu-id="f01b2-120">Wechseln Sie in einem Webbrowser zu dieser URL, https://youtu.be/wYrRCRphrp0 und rufen Sie den Einbettungscode für das Video ab.</span><span class="sxs-lookup"><span data-stu-id="f01b2-120">In a Web browser, go to this URL https://youtu.be/wYrRCRphrp0 and get the embed code for the video.</span></span> 
6.  <span data-ttu-id="f01b2-121">Wählen Sie im SharePoint-Webpart Einbettungscode hinzufügen aus, und fügen Sie ihn dann in das Feld embed ein.</span><span class="sxs-lookup"><span data-stu-id="f01b2-121">In the SharePoint Web part, select Add Embed code and then paste it into the Embed box.</span></span> 
7.  <span data-ttu-id="f01b2-122">Wählen Sie im rechten Feld Neues Webpart hinzufügen aus, und wählen Sie dann Text aus.</span><span class="sxs-lookup"><span data-stu-id="f01b2-122">In the right-hand box, select Add a new web part, and then select Text.</span></span> 
8.  <span data-ttu-id="f01b2-123">Wechseln Sie in einem Webbrowser zu dieser URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b und kopieren Sie den Test it!</span><span class="sxs-lookup"><span data-stu-id="f01b2-123">In a Web browser, go to this URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b and copy the Try it!</span></span> <span data-ttu-id="f01b2-124">Anweisungen auf der Seite aus, und fügen Sie Sie in das Text Webpart ein.</span><span class="sxs-lookup"><span data-stu-id="f01b2-124">Instructions from the page and paste them into the Text Web part.</span></span> <span data-ttu-id="f01b2-125">Die Seite sollte wie folgt aussehen.</span><span class="sxs-lookup"><span data-stu-id="f01b2-125">Your page should look like the following.</span></span> 

![Seite einbetten](media/clo365teamscommandbox.png)

9.  <span data-ttu-id="f01b2-127">Klicken Sie auf **veröffentlichen**, und kopieren Sie dann die URL der Seite, und fügen Sie Sie in Notepad ein.</span><span class="sxs-lookup"><span data-stu-id="f01b2-127">Click **Publish**, and then copy the URL of the page and paste it in Notepad</span></span>

#### <a name="step-2-create-the-playlist"></a><span data-ttu-id="f01b2-128">Schritt 2: Erstellen der Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="f01b2-128">Step 2: Create the Playlist</span></span>

1. <span data-ttu-id="f01b2-129">Navigieren Sie zur Seite **benutzerdefinierte Lern Verwaltung** in ihrer Websiteumgebung.</span><span class="sxs-lookup"><span data-stu-id="f01b2-129">Navigate to the **Custom Learning Administration** page in your site experience.</span></span>
<span data-ttu-id="f01b2-130">![custom_admin.png](media/custom_admin.png)</span><span class="sxs-lookup"><span data-stu-id="f01b2-130">![custom_admin.png](media/custom_admin.png)</span></span>
1. <span data-ttu-id="f01b2-131">Sicherstellen, dass **Kategorie** ausgewählt ist</span><span class="sxs-lookup"><span data-stu-id="f01b2-131">Make sure **Category** is selected</span></span> 
1. <span data-ttu-id="f01b2-132">Klicken Sie auf die Kategorie, in der Sie Ihre neue Wiedergabeliste anzeigen möchten.</span><span class="sxs-lookup"><span data-stu-id="f01b2-132">Click on the category where you'd like your new playlist to appear</span></span>
1. <span data-ttu-id="f01b2-133">Klicken Sie neben dem Namen der Kategorie auf das Plus-Symbol ![custom_addplay.png](media/custom_addplay.png)</span><span class="sxs-lookup"><span data-stu-id="f01b2-133">Next to the category name, click on the plus symbol ![custom_addplay.png](media/custom_addplay.png)</span></span>

1. <span data-ttu-id="f01b2-134">Geben Sie die Werte wie im folgenden Beispiel gezeigt ein, und wählen Sie **Erstellen**aus.</span><span class="sxs-lookup"><span data-stu-id="f01b2-134">Fill in the values as shown in the example below and select **Create**.</span></span> 
<span data-ttu-id="f01b2-135">![custom_details.png](media/custom_details.png)</span><span class="sxs-lookup"><span data-stu-id="f01b2-135">![custom_details.png](media/custom_details.png)</span></span>
- <span data-ttu-id="f01b2-136">**Title** – Anzeigename der Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="f01b2-136">**Title** - Display name of the playlist</span></span>
- <span data-ttu-id="f01b2-137">**Beschreibung** – Informationen zu den Vorgehensweise</span><span class="sxs-lookup"><span data-stu-id="f01b2-137">**Description** - Information about what will be learned</span></span>
- <span data-ttu-id="f01b2-138">**Kategorie** -preselected basierend auf Ihrer anfänglichen Auswahl</span><span class="sxs-lookup"><span data-stu-id="f01b2-138">**Category** - Preselected based on your initial selection</span></span>
- <span data-ttu-id="f01b2-139">**Unterkategorie** – vorab ausgewählt basierend auf Ihrer anfänglichen Auswahl</span><span class="sxs-lookup"><span data-stu-id="f01b2-139">**Sub Category** - Preselected based on your intial selection</span></span>
- <span data-ttu-id="f01b2-140">**Technologie** – je nach Bedarf auswählen</span><span class="sxs-lookup"><span data-stu-id="f01b2-140">**Technology** - Select as applicable</span></span>
- <span data-ttu-id="f01b2-141">**Stufe** – Anfänger, Intermidate oder erweitert</span><span class="sxs-lookup"><span data-stu-id="f01b2-141">**Level** - Beginner, Intermidate or Advanced</span></span>
- <span data-ttu-id="f01b2-142">Ziel **Gruppe** : auf diese Weise können Sie Inhalte basierend auf einer vordefinierten Liste von Rollen, die von Microsoft bereitgestellt werden, gezielt anfertigen.</span><span class="sxs-lookup"><span data-stu-id="f01b2-142">**Audience** - This allows you to target content based on a pre-defined list of roles provided by Microsoft.</span></span>

6. <span data-ttu-id="f01b2-143">Klicken Sie auf **Detail speichern**</span><span class="sxs-lookup"><span data-stu-id="f01b2-143">Click **Save Detail**</span></span>

> [!TIP]
> <span data-ttu-id="f01b2-144">Sie können das Symbolbild für Ihre Wiedergabeliste anpassen.</span><span class="sxs-lookup"><span data-stu-id="f01b2-144">You can customize the icon image for your playlist.</span></span>  <span data-ttu-id="f01b2-145">Klicken Sie auf das Bildsymbol, und fügen Sie eine URL eines zuvor hochgeladenen Bilds ein.</span><span class="sxs-lookup"><span data-stu-id="f01b2-145">Click the image icon and insert an URL of a previously uploaded image.</span></span>  <span data-ttu-id="f01b2-146">Stellen Sie sicher, dass sich das Bild in der benutzerdefinierten Lernwebsite Sammlung oder an einem anderen Speicherort befindet, auf das alle Benutzer Zugriff auf die Datei erhalten.</span><span class="sxs-lookup"><span data-stu-id="f01b2-146">Make sure the image is located within the Custom Learning site collection or in another location that all users will have access to the file.</span></span>  
<span data-ttu-id="f01b2-147">![custom_image.png](media/custom_image.png)</span><span class="sxs-lookup"><span data-stu-id="f01b2-147">![custom_image.png](media/custom_image.png)</span></span>

#### <a name="step-3-add-assets-to-the-playlist"></a><span data-ttu-id="f01b2-148">Schritt 3: Hinzufügen von Objekten zur Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="f01b2-148">Step 3: Add assets to the playlist</span></span>
<span data-ttu-id="f01b2-149">In diesem Schritt fügen Sie vorhandene Objekte aus Microsoft und die SharePoint-Seite, die Sie erstellt haben, zur Wiedergabeliste hinzu.</span><span class="sxs-lookup"><span data-stu-id="f01b2-149">In this step, you’ll add existing assets from Microsoft and the SharePoint page you created to the playlist.</span></span> 

1. <span data-ttu-id="f01b2-150">Nachdem Sie die Details für Ihre Wiedergabeliste gespeichert haben, können Sie die Suche nach vorhandenen Objekten verwenden.</span><span class="sxs-lookup"><span data-stu-id="f01b2-150">Once you have saved the details for your Playlist you can use the Search for Existing Assets.</span></span>
1. <span data-ttu-id="f01b2-151">**Geben Sie in einen beliebigen Suchbegriff** ein, um eine Liste der vordefinierten Objekte anzuzeigen, die in anderen Wiedergabelisten verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="f01b2-151">**Enter in any search term** to see a list of predefined assets that are available from other playlists.</span></span> <span data-ttu-id="f01b2-152">**Klicken Sie auf den Namen** eines Objekts, um es in Ihre neue Wiedergabeliste einzuschließen.</span><span class="sxs-lookup"><span data-stu-id="f01b2-152">**Click on the name** of an asset to include it in your new playlist.</span></span>
<span data-ttu-id="f01b2-153">![custom_slist.png](media/custom_slist.png)</span><span class="sxs-lookup"><span data-stu-id="f01b2-153">![custom_slist.png](media/custom_slist.png)</span></span>

<span data-ttu-id="f01b2-154">Sie können auch die zuvor erstellte SharePoint-Seite hinzufügen oder eine von Grund auf neu in der Benutzeroberfläche erstellen.</span><span class="sxs-lookup"><span data-stu-id="f01b2-154">You can also add the SharePoint page you created earlier or create one from scratch in the experience.</span></span>

1. <span data-ttu-id="f01b2-155">Klicken Sie auf die Option " **Neues Objekt** " im Dialogfeld "Wiedergabelisten Objekte"</span><span class="sxs-lookup"><span data-stu-id="f01b2-155">Click on the **New Asset** option in the Playlist Assets dialog</span></span>
1. <span data-ttu-id="f01b2-156">Geben Sie Ihrem Objekt einen **Titel**.</span><span class="sxs-lookup"><span data-stu-id="f01b2-156">Give your asset a **Title**.</span></span> <span data-ttu-id="f01b2-157">Nach der Eingabe werden weitere Optionen angezeigt ![custom_newpage.png](media/custom_newpage.png)</span><span class="sxs-lookup"><span data-stu-id="f01b2-157">Once entered, additional options will display ![custom_newpage.png](media/custom_newpage.png)</span></span>
1. <span data-ttu-id="f01b2-158">Sie können nun eine neue Anlage Seite in SharePoint Online erstellen oder die URL einer vorhandenen Seite eingeben, um Sie Ihrer benutzerdefinierten Wiedergabeliste hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="f01b2-158">You can now create a new asset page in SharePoint Online or enter in the URL of an existing page to add it to your custom playlist.</span></span> 
1. <span data-ttu-id="f01b2-159">**Kategorien**-, **Unterkategorie** -und **Technologie** Felder werden basierend auf Ihrer vorherigen Auswahl für diese Wiedergabeliste vorab ausgefüllt.</span><span class="sxs-lookup"><span data-stu-id="f01b2-159">**Category**, **Sub Category** and **Technology** fields will be pre-populated based on your previous selections for this playlist.</span></span>
1. <span data-ttu-id="f01b2-160">Treffen Sie die entsprechenden Auswahlmöglichkeiten für Ebene und Zielgruppe für diese einzelne Ressource.</span><span class="sxs-lookup"><span data-stu-id="f01b2-160">Make the appropriate selections for Level and Audience for this individual asset.</span></span>  
1. <span data-ttu-id="f01b2-161">Klicken Sie auf **Objekt speichern** , um es der benutzerdefinierten Wiedergabeliste hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="f01b2-161">Click **Save Asset** to add it to the custom playlist</span></span>
1. <span data-ttu-id="f01b2-162">Wiederholen Sie diese Schritte, entweder durchsuchen oder Hinzufügen einzelner Seiten, bis Ihre Wiedergabeliste abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="f01b2-162">Repeat these steps, either searching or adding individual pages, until your playlist is complete.</span></span> 
1. <span data-ttu-id="f01b2-163">Klicken Sie auf **Playlist schließen** , um zu speichern</span><span class="sxs-lookup"><span data-stu-id="f01b2-163">Click **Close Playlist** to save</span></span>

<span data-ttu-id="f01b2-164">Ihre Wiedergabeliste mit diesem Inhalt ist jetzt überall verfügbar, wo Sie das benutzerdefinierte Lern Webpart installiert/eingebettet haben.</span><span class="sxs-lookup"><span data-stu-id="f01b2-164">Your playlist with this content will now be available anywhere you have installed / embedded the Custom Learning webpart.</span></span> 

> [!NOTE]
> <span data-ttu-id="f01b2-165">Wenn Sie einen Fehler gemacht haben, nachdem Sie die Wiedergabeliste geschlossen haben, können Sie Sie aus der Kategorie löschen, indem Sie auf das X neben dem Namen der Wiedergabeliste klicken.</span><span class="sxs-lookup"><span data-stu-id="f01b2-165">If you make a mistake once you have closed the playlist, you can delete it from the category by clicking the X next to the playlist name.</span></span>  

#### <a name="things-to-think-about"></a><span data-ttu-id="f01b2-166">Dinge, über die Sie nachdenken sollten</span><span class="sxs-lookup"><span data-stu-id="f01b2-166">Things to Think About</span></span>

<span data-ttu-id="f01b2-167">Benutzerdefinierte Wiedergabelisten können verwendet werden, um Ihre Endbenutzer in einer Vielzahl von Aufgaben zu unterstützen.</span><span class="sxs-lookup"><span data-stu-id="f01b2-167">Custom playlists can be used to assist your end users in a variety of tasks.</span></span>  <span data-ttu-id="f01b2-168">Haben Sie ein Formular für die Auszeit von Anfragen?</span><span class="sxs-lookup"><span data-stu-id="f01b2-168">Do you have a time off request form?</span></span>  <span data-ttu-id="f01b2-169">Ein Formular zum Anfordern von Hardwaregeräten?</span><span class="sxs-lookup"><span data-stu-id="f01b2-169">A form to request hardware equipment?</span></span>  <span data-ttu-id="f01b2-170">Vorhandene Schulungsressourcen können in die Benutzeroberfläche programmiert werden.</span><span class="sxs-lookup"><span data-stu-id="f01b2-170">Any existing training assets can be programmed into the experience.</span></span>  

## <a name="share-playlists"></a><span data-ttu-id="f01b2-171">Freigeben von Wiedergabelisten</span><span class="sxs-lookup"><span data-stu-id="f01b2-171">Share Playlists</span></span>

1. <span data-ttu-id="f01b2-172">Navigieren zu einer beliebigen Wiedergabeliste innerhalb des Webpart-oder Website Erlebnisses</span><span class="sxs-lookup"><span data-stu-id="f01b2-172">Navigate to any playlist within the webpart or site experience</span></span>
1. <span data-ttu-id="f01b2-173">In der linken oberen Ecke werden drei Symbole angezeigt.</span><span class="sxs-lookup"><span data-stu-id="f01b2-173">In the upper left hand corner you will see three icons</span></span>
1. <span data-ttu-id="f01b2-174">Klicken Sie auf das Symbol, das einen Link darstellt.</span><span class="sxs-lookup"><span data-stu-id="f01b2-174">Click on the icon representing a link</span></span>
1. <span data-ttu-id="f01b2-175">Kopieren der URL in die Wiedergabeliste</span><span class="sxs-lookup"><span data-stu-id="f01b2-175">Copy the URL to the playlist</span></span>

<span data-ttu-id="f01b2-176">![share.png](media/share.png) diese URL kann nun in Ihre Websitenavigation eingefügt oder in anderer Kommunikation verwendet werden, um Ihre Mitarbeiter direkt in diese Wiedergabeliste zu übernehmen.</span><span class="sxs-lookup"><span data-stu-id="f01b2-176">![share.png](media/share.png) This URL can now be inserted in your site navigation or utilized in other communications to take your employees directly to that playlist.</span></span> 

### <a name="next-steps---drive-adoption"></a><span data-ttu-id="f01b2-177">Nächste Schritte – [Einführung in die Festplatte](driveadoption.md)</span><span class="sxs-lookup"><span data-stu-id="f01b2-177">Next Steps - [Drive Adoption](driveadoption.md)</span></span>
