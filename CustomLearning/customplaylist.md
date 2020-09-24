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
# <a name="customize-and-share-playlists"></a>Anpassen und Freigeben von Wiedergabelisten

## <a name="create-a-playlist"></a>Erstellen einer Wiedergabeliste

Eine Wiedergabeliste entspricht "Assets". Ein "Asset" ist eine SharePoint-Seite oder ein vorhandenes Element von Microsoft-Schulungsinhalten. Wenn Sie eine Wiedergabeliste erstellen, wählen Sie Objekte aus, die zusammen gehen, um einen Lernpfad für Ihren Benutzer zu erstellen.  

Der Vorteil des Hinzufügens von SharePoint-Seiten ist, dass Sie SharePoint-Seiten mit einem YouTube-Videos oder Videos in Ihrer Organisation gehostet erstellen können. Sie können auch Seiten mit Formularen oder anderen Office 365 Inhalten erstellen.  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a>Schritt 1: Erstellen einer SharePoint-Seite für Ihre Wiedergabeliste
In diesem Beispiel erstellen wir zunächst eine SharePoint-Seite, die der Wiedergabeliste hinzugefügt werden soll. Wir erstellen eine Seite mit einem YouTube-Video-Webpart und einem Text-WebPart.  Bei diesen Anweisungen wird davon ausgegangen, dass Sie den SharePoint Online Dienst verwenden. 

#### <a name="create-a-new-page"></a>Eine neue Seite erstellen
1.  Wählen Sie das Menü Einstellungen > Websiteinhalte > Website Seiten > Seite neue > Site aus.
2.  Geben Sie im Bereich Titel den Befehl Teams verwenden ein.
3.  Wählen Sie den Abschnitt neuen Abschnitt hinzufügen aus, und wählen Sie dann zwei Spalten aus.

![zweispaltige hinzufügen](media/clo365addtwocolumn.png)

4.  Wählen Sie im linken Feld Neues Webpart hinzufügen aus, und wählen Sie dann einbetten aus. 
5.  Wechseln Sie in einem Webbrowser zu dieser URL, https://youtu.be/wYrRCRphrp0 und rufen Sie den Einbettungscode für das Video ab. 
6.  Wählen Sie im SharePoint-Webpart Einbettungscode hinzufügen aus, und fügen Sie ihn dann in das Feld embed ein. 
7.  Wählen Sie im rechten Feld Neues Webpart hinzufügen aus, und wählen Sie dann Text aus. 
8.  Wechseln Sie in einem Webbrowser zu dieser URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b und kopieren Sie den Test it! Anweisungen auf der Seite aus, und fügen Sie Sie in das Text Webpart ein. Die Seite sollte wie folgt aussehen. 

![Seite einbetten](media/clo365teamscommandbox.png)

9.  Klicken Sie auf **veröffentlichen**, und kopieren Sie dann die URL der Seite, und fügen Sie Sie in Notepad ein.

#### <a name="step-2-create-the-playlist"></a>Schritt 2: Erstellen der Wiedergabeliste

1. Navigieren Sie zur Seite **benutzerdefinierte Lern Verwaltung** in ihrer Websiteumgebung.
![custom_admin.png](media/custom_admin.png)
1. Sicherstellen, dass **Kategorie** ausgewählt ist 
1. Klicken Sie auf die Kategorie, in der Sie Ihre neue Wiedergabeliste anzeigen möchten.
1. Klicken Sie neben dem Namen der Kategorie auf das Plus-Symbol ![custom_addplay.png](media/custom_addplay.png)

1. Geben Sie die Werte wie im folgenden Beispiel gezeigt ein, und wählen Sie **Erstellen**aus. 
![custom_details.png](media/custom_details.png)
- **Title** – Anzeigename der Wiedergabeliste
- **Beschreibung** – Informationen zu den Vorgehensweise
- **Kategorie** -preselected basierend auf Ihrer anfänglichen Auswahl
- **Unterkategorie** – vorab ausgewählt basierend auf Ihrer anfänglichen Auswahl
- **Technologie** – je nach Bedarf auswählen
- **Stufe** – Anfänger, Intermidate oder erweitert
- Ziel **Gruppe** : auf diese Weise können Sie Inhalte basierend auf einer vordefinierten Liste von Rollen, die von Microsoft bereitgestellt werden, gezielt anfertigen.

6. Klicken Sie auf **Detail speichern**

> [!TIP]
> Sie können das Symbolbild für Ihre Wiedergabeliste anpassen.  Klicken Sie auf das Bildsymbol, und fügen Sie eine URL eines zuvor hochgeladenen Bilds ein.  Stellen Sie sicher, dass sich das Bild in der benutzerdefinierten Lernwebsite Sammlung oder an einem anderen Speicherort befindet, auf das alle Benutzer Zugriff auf die Datei erhalten.  
![custom_image.png](media/custom_image.png)

#### <a name="step-3-add-assets-to-the-playlist"></a>Schritt 3: Hinzufügen von Objekten zur Wiedergabeliste
In diesem Schritt fügen Sie vorhandene Objekte aus Microsoft und die SharePoint-Seite, die Sie erstellt haben, zur Wiedergabeliste hinzu. 

1. Nachdem Sie die Details für Ihre Wiedergabeliste gespeichert haben, können Sie die Suche nach vorhandenen Objekten verwenden.
1. **Geben Sie in einen beliebigen Suchbegriff** ein, um eine Liste der vordefinierten Objekte anzuzeigen, die in anderen Wiedergabelisten verfügbar sind. **Klicken Sie auf den Namen** eines Objekts, um es in Ihre neue Wiedergabeliste einzuschließen.
![custom_slist.png](media/custom_slist.png)

Sie können auch die zuvor erstellte SharePoint-Seite hinzufügen oder eine von Grund auf neu in der Benutzeroberfläche erstellen.

1. Klicken Sie auf die Option " **Neues Objekt** " im Dialogfeld "Wiedergabelisten Objekte"
1. Geben Sie Ihrem Objekt einen **Titel**. Nach der Eingabe werden weitere Optionen angezeigt ![custom_newpage.png](media/custom_newpage.png)
1. Sie können nun eine neue Anlage Seite in SharePoint Online erstellen oder die URL einer vorhandenen Seite eingeben, um Sie Ihrer benutzerdefinierten Wiedergabeliste hinzuzufügen. 
1. **Kategorien**-, **Unterkategorie** -und **Technologie** Felder werden basierend auf Ihrer vorherigen Auswahl für diese Wiedergabeliste vorab ausgefüllt.
1. Treffen Sie die entsprechenden Auswahlmöglichkeiten für Ebene und Zielgruppe für diese einzelne Ressource.  
1. Klicken Sie auf **Objekt speichern** , um es der benutzerdefinierten Wiedergabeliste hinzuzufügen.
1. Wiederholen Sie diese Schritte, entweder durchsuchen oder Hinzufügen einzelner Seiten, bis Ihre Wiedergabeliste abgeschlossen ist. 
1. Klicken Sie auf **Playlist schließen** , um zu speichern

Ihre Wiedergabeliste mit diesem Inhalt ist jetzt überall verfügbar, wo Sie das benutzerdefinierte Lern Webpart installiert/eingebettet haben. 

> [!NOTE]
> Wenn Sie einen Fehler gemacht haben, nachdem Sie die Wiedergabeliste geschlossen haben, können Sie Sie aus der Kategorie löschen, indem Sie auf das X neben dem Namen der Wiedergabeliste klicken.  

#### <a name="things-to-think-about"></a>Dinge, über die Sie nachdenken sollten

Benutzerdefinierte Wiedergabelisten können verwendet werden, um Ihre Endbenutzer in einer Vielzahl von Aufgaben zu unterstützen.  Haben Sie ein Formular für die Auszeit von Anfragen?  Ein Formular zum Anfordern von Hardwaregeräten?  Vorhandene Schulungsressourcen können in die Benutzeroberfläche programmiert werden.  

## <a name="share-playlists"></a>Freigeben von Wiedergabelisten

1. Navigieren zu einer beliebigen Wiedergabeliste innerhalb des Webpart-oder Website Erlebnisses
1. In der linken oberen Ecke werden drei Symbole angezeigt.
1. Klicken Sie auf das Symbol, das einen Link darstellt.
1. Kopieren der URL in die Wiedergabeliste

![share.png](media/share.png) diese URL kann nun in Ihre Websitenavigation eingefügt oder in anderer Kommunikation verwendet werden, um Ihre Mitarbeiter direkt in diese Wiedergabeliste zu übernehmen. 

### <a name="next-steps---drive-adoption"></a>Nächste Schritte – [Einführung in die Festplatte](driveadoption.md)
