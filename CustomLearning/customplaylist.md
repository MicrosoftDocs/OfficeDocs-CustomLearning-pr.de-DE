---
author: karuanag
ms.author: karuanag
title: Anpassen und Freigeben von Wiedergabelisten
ms.date: 02/10/2019
description: Erstellen benutzerdefinierter Wiedergabelisten aus vorhandenen Inhalten oder neuen SharePoint-Seiten
ms.openlocfilehash: d330b6e401c9020eb68877bc8a132350811a2f31
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32056401"
---
# <a name="customize-and-share-playlists"></a>Anpassen und Freigeben von Wiedergabelisten

## <a name="create-a-playlist"></a>Erstellen einer Wiedergabeliste

Eine Wiedergabeliste ist die Einhaltung von "Assets". Ein "Asset" ist eine SharePoint-Seite oder ein vorhandenes Element von Microsoft-Schulungsinhalten. Wenn Sie eine Wiedergabeliste erstellen, wählen Sie Objekte aus, die gemeinsam einen Lernpfad für Ihren Benutzer erstellen.  

Der Vorteil beim Hinzufügen von SharePoint-Seiten besteht darin, dass Sie SharePoint-Seiten mit YouTube-Videos oder-Videos erstellen können, die in Ihrer Organisation gehostet werden. Sie können auch Seiten mit Formularen oder anderen Office 365-Inhalten erstellen.  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a>Schritt 1: Erstellen einer SharePoint-Seite für Ihre Wiedergabeliste
In diesem Beispiel erstellen wir zunächst eine SharePoint-Seite, die der Wiedergabeliste hinzugefügt werden soll. Wir erstellen eine Seite mit einem YouTube-Video-Webpart und einem Text WebPart.  Bei diesen Anweisungen wird davon ausgegangen, dass Sie den SharePoint Online-Dienst verwenden. 

#### <a name="create-a-new-page"></a>Eine neue Seite erstellen
1.  Wählen Sie das Menü Einstellungen > Site Contents > Site Pages > New > Site Page aus.
2.  Geben Sie im Bereich Titel den Befehl Teams verwenden ein.
3.  Wählen Sie den Abschnitt neuen hinzufügen aus, und wählen Sie dann zwei Spalten aus.

![zwei Spalten hinzufügen](media/clo365addtwocolumn.png)

4.  Klicken Sie im linken Feld auf neues Webpart hinzufügen, und wählen Sie dann einBetten aus. 
5.  Wechseln Sie in einem Webbrowser zu dieser URL https://youtu.be/wYrRCRphrp0 , und rufen Sie den embed-Code für das Video ab. 
6.  Wählen Sie im SharePoint-Webpart embed-Code hinzufügen aus, und fügen Sie ihn dann in das Feld embed ein. 
7.  Klicken Sie im rechten Feld auf neues Webpart hinzufügen, und wählen Sie dann Text aus. 
8.  Wechseln Sie in einem Webbrowser zu dieser URL: https://support.office.com/en-us/article/13c4e429-7324-4886-b377-5dbed539193b , und kopieren Sie die try it! Anweisungen auf der Seite und fügen Sie Sie in das Text Webpart ein. Ihre Seite sollte wie folgt aussehen. 

![Seite einBetten](media/clo365teamscommandbox.png)

9.  Klicken Sie auf **veröffentlichen**, und kopieren Sie dann die URL der Seite, und fügen Sie Sie in Notepad ein.

#### <a name="step-2-create-the-playlist"></a>Schritt 2: Erstellen der Wiedergabeliste

1. Navigieren Sie zur **benutzerdefinierten Learning Administration** -Seite in der Websiteumgebung.
![custom_admin. png](media/custom_admin.png)
1. Stellen Sie sicher, dass **Kategorie** ausgewählt ist. 
1. Klicken Sie auf die Kategorie, in der die neue Wiedergabeliste angezeigt werden soll.
1. Klicken Sie neben dem Namen der Kategorie auf das Pluszeichen ![custom_addplay. png.](media/custom_addplay.png)

1. Geben Sie die Werte wie im folgenden Beispiel ein, und wählen Sie **Erstellen**aus. 
![custom_details. png](media/custom_details.png)
- **Title** – Anzeigename der Wiedergabeliste
- **Beschreibung** – Informationen zu den erlernten
- **Kategorie** -vorab ausgewählt basierend auf der anfänglichen Auswahl
- **Unterkategorie** – ausgewählt basierend auf Ihrer anfänglichen Auswahl
- **Technologie** – Auswahl nach Bedarf
- **Stufe** – Anfänger, Intermidate oder erweitert
- Ziel **Gruppe** – auf diese Weise können Sie Inhalte basierend auf einer vordefinierten Liste von Rollen, die von Microsoft bereitgestellt werden, ausrichten.

6. Klicken Sie auf **Details speichern**

> [!TIP]
> Sie können das Symbolbild für Ihre Wiedergabeliste anpassen.  Klicken Sie auf das Bildsymbol, und fügen Sie eine URL eines zuvor hochgeladenen Bilds ein.  Stellen Sie sicher, dass sich das Bild in der benutzerdefinierten Learning-Websitesammlung oder an einem anderen Speicherort befindet, auf den alle Benutzer Zugriff auf die Datei haben.  
![custom_image. png](media/custom_image.png)

#### <a name="step-3-add-assets-to-the-playlist"></a>Schritt 3: Hinzufügen von Objekten zur Wiedergabeliste
In diesem Schritt fügen Sie vorhandene Objekte aus Microsoft und die von Ihnen erstellte SharePoint-Seite der Wiedergabeliste hinzu. 

1. Nachdem Sie die Details für Ihre Wiedergabeliste gespeichert haben, können Sie die Suche nach vorhandenen Objekten verwenden.
1. **Geben Sie in einen beliebigen Suchbegriff** ein, um eine Liste der vordefinierten Objekte anzuzeigen, die von anderen Wiedergabelisten zur Verfügung stehen. **Klicken Sie auf den Namen** eines Objekts, um es in die neue Wiedergabeliste einzufügen.
![custom_slist. png](media/custom_slist.png)

Sie können auch die zuvor erstellte SharePoint-Seite hinzufügen oder eine von Grund auf neu erstellen.

1. Klicken Sie im Dialogfeld "Wiedergabelisten Objekte" auf die Option " **Neues Element** ".
1. Geben Sie Ihrem Asset einen **Titel**. Nach der Eingabe werden zusätzliche Optionen custom_newpage ![. png angezeigt.](media/custom_newpage.png)
1. Sie können jetzt eine neue Objekt Seite in SharePoint Online erstellen oder die URL einer vorhandenen Seite eingeben, um Sie Ihrer benutzerdefinierten Wiedergabeliste hinzuzufügen. 
1. **Kategorien**-, **Unterkategorie** -und **Technologie** Felder werden basierend auf Ihrer vorherigen Auswahl für diese Wiedergabeliste vorab aufgefüllt.
1. Treffen Sie die richtige Auswahl für Ebene und Zielgruppe für dieses einzelne Objekt.  
1. Klicken Sie auf **Ressource speichern** , um Sie der benutzerdefinierten Wiedergabeliste hinzuzufügen.
1. Wiederholen Sie diese Schritte, indem Sie einzelne Seiten durchsuchen oder hinzufügen, bis die Wiedergabeliste abgeschlossen ist. 
1. Klicken Sie auf **Wiedergabeliste** zum Speichern Beenden

Ihre Wiedergabeliste mit diesem Inhalt ist jetzt verfügbar, wenn Sie das benutzerdefinierte Lern Webpart installiert/eingebettet haben. 

> [!NOTE]
> Wenn Sie einen Fehler gemacht haben, nachdem Sie die Wiedergabeliste geschlossen haben, können Sie Sie aus der Kategorie löschen, indem Sie auf das X neben dem Namen der Wiedergabeliste klicken.  

#### <a name="things-to-think-about"></a>Zu berücksichtigende Aspekte

Benutzerdefinierte Wiedergabelisten können verwendet werden, um Ihre Endbenutzer bei einer Vielzahl von Aufgaben zu unterstützen.  Haben Sie ein Formular für die Ausfallszeit?  Ein Formular zum Anfordern von Hardwaregeräten?  Vorhandene Trainings Objekte können in die Umgebung einprogrammiert werden.  

## <a name="share-playlists"></a>Freigeben von Wiedergabelisten

1. Navigieren Sie zu einer beliebigen Wiedergabeliste innerhalb der Webpart-oder Websiteumgebung.
1. In der oberen linken Ecke werden drei Symbole angezeigt.
1. Klicken Sie auf das Symbol, das einen Link darstellt.
1. Kopieren der URL in die Wiedergabeliste

![share. png](media/share.png) diese URL kann jetzt in Ihre Websitenavigation eingefügt oder in anderer Kommunikation verwendet werden, um Ihre Mitarbeiter direkt zu dieser Wiedergabeliste zu übertragen. 

### <a name="next-steps---drive-adoptiondriveadoptionmd"></a>Nächste Schritte- [Einführung](driveadoption.md)
