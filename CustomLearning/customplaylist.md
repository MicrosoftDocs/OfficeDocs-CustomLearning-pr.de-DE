---
author: karuanag
ms.author: karuanag
manager: alexb
title: Anpassen und Freigeben von Wiedergabelisten
ms.date: 02/10/2019
description: Erstellen benutzerdefinierter Wiedergabelisten aus vorhandenen Inhalten oder neuen SharePoint-Seiten
ms.service: sharepoint-online
audience: itpro
ms.topic: article
ms.openlocfilehash: 31a0e5524181d26f4d62ae7206636c9e553b6f8f
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000211"
---
# <a name="customize-and-share-playlists"></a>Anpassen und Freigeben von Wiedergabelisten

## <a name="create-a-playlist"></a>Erstellen einer Wiedergabeliste

Eine Wiedergabeliste ist eine Komplizenschaft von "Assets". Ein "Objekt" ist eine SharePoint-Seite oder ein vorhandenes Element von Microsoft-Schulungsinhalten. Wenn Sie eine Wiedergabeliste erstellen, wählen Sie Ressourcen aus, die zusammengehen, um einen Lernpfad für Ihren Benutzer zu erstellen.  

Der Vorteil des Hinzufügens von SharePoint-Seiten besteht in der Erstellung von SharePoint-Seiten mit youTube-Videos oder -Videos, die in Ihrer Organisation gehostet werden. Sie können auch Seiten mit Formularen oder anderen Office 365-Inhalten erstellen.  

#### <a name="step-1-create-a-sharepoint-page-for-your-playlist"></a>Schritt 1: Erstellen einer SharePoint-Seite für Ihre Wiedergabeliste
In diesem Beispiel erstellen wir zunächst eine SharePoint-Seite, die der Wiedergabeliste hinzugefügt werden soll. Wir erstellen eine Seite mit einem YouTube-Videowebteil und einem Text-Web part.  In diesen Anweisungen wird davon ausgegangen, dass Sie den SharePoint Online-Dienst verwenden. 

#### <a name="create-a-new-page"></a>Eine neue Seite erstellen
1.  Wählen Sie das Menü Einstellungen > Websiteinhalte > Websiteseiten > Neue > Websiteseite aus.
2.  Geben Sie im Titelbereich das Befehlsfeld Teams verwenden ein.
3.  Wählen Sie den Abschnitt Hinzufügen eines neuen Abschnitts aus, und wählen Sie dann Zwei Spalten aus.

![Hinzufügen von zwei Spalten](media/clo365addtwocolumn.png)

4.  Wählen Sie im linken Feld Hinzufügen eines neuen Webteils aus, und wählen Sie dann Einbetten aus. 
5.  Wechseln Sie in einem Webbrowser zu dieser https://youtu.be/wYrRCRphrp0 URL, und erhalten Sie den Einbettungscode für das Video. 
6.  Wählen Sie im SharePoint-Webteil Code hinzufügen aus, und fügen Sie ihn dann in das Feld Einbetten ein. 
7.  Wählen Sie im rechten Feld Hinzufügen eines neuen Webteils aus, und wählen Sie dann Text aus. 
8.  Wechseln Sie in einem Webbrowser zu dieser URL: https://support.office.com/article/13c4e429-7324-4886-b377-5dbed539193b und kopieren Sie das Probieren Sie es! Anweisungen von der Seite, und fügen Sie sie in das Textwebteil ein. Ihre Seite sollte wie folgt aussehen. 
![Einbettungsseite](media/clo365teamscommandbox.png)
9.  Klicken **Sie auf** Veröffentlichen, und kopieren Sie dann die URL der Seite, und fügen Sie sie in Editor ein.

#### <a name="step-2-create-the-playlist"></a>Schritt 2: Erstellen der Wiedergabeliste

1. Navigieren Sie zur **Seite Benutzerdefinierte Lernverwaltung** in Ihrer Websiteumgebung.
![Bildschirm, auf dem Sie Benutzerdefinierte Lernverwaltung auswählen.](media/custom_admin.png)
1. Sicherstellen, **dass Kategorie** ausgewählt ist 
1. Klicken Sie auf die Kategorie, in der Ihre neue Wiedergabeliste angezeigt werden soll
1. Klicken Sie neben dem Kategorienamen auf das Plussymbol Fenster mit der ![ Option Kategorie und dem Pluszeichen hervorgehoben.](media/custom_addplay.png)

1. Füllen Sie die Werte aus, wie im folgenden Beispiel gezeigt, und wählen Sie **Erstellen aus.** 
![Seite, auf der Sie Wiedergabelistendetails eingeben.](media/custom_details.png)
- **Titel** – Anzeigename der Wiedergabeliste
- **Beschreibung** – Informationen zu den Gelernten
- **Kategorie** – Basierend auf Ihrer ursprünglichen Auswahl vorgewählt
- **Unterkategorie** – Basierend auf Ihrer Initialauswahl vorab ausgewählt
- **Technologie** – Wählen Sie ggf. aus
- **Level** – Anfänger, Intermidate oder Fortgeschrittene
- **Zielgruppe** – Auf diese Weise können Sie Inhalte basierend auf einer vordefinierten Liste von Rollen, die von Microsoft bereitgestellt werden, als Ziel verwenden.

6. Klicken Sie **auf Details speichern**

> [!TIP]
> Sie können das Symbolbild für Ihre Wiedergabeliste anpassen.  Klicken Sie auf das Bildsymbol, und fügen Sie eine URL eines zuvor hochgeladenen Bilds ein.  Stellen Sie sicher, dass sich das Bild in der Benutzerdefinierten Lernwebsitesammlung oder an einem anderen Speicherort befindet, an dem alle Benutzer Zugriff auf die Datei haben.  
![Wählen Sie ein Bildfenster aus.](media/custom_image.png)

#### <a name="step-3-add-assets-to-the-playlist"></a>Schritt 3: Hinzufügen von Ressourcen zur Wiedergabeliste
In diesem Schritt fügen Sie der Wiedergabeliste vorhandene Objekte von Microsoft und die von Ihnen erstellte SharePoint-Seite hinzu. 

1. Nachdem Sie die Details für Ihre Wiedergabeliste gespeichert haben, können Sie die Suche nach vorhandenen Ressourcen verwenden.
1. **Geben Sie einen beliebigen Suchbegriff** ein, um eine Liste vordefinierter Objekte zu sehen, die in anderen Wiedergabelisten verfügbar sind. **Klicken Sie auf den Namen** einer Ressource, um sie in Ihre neue Wiedergabeliste zu schließen.<br/>
![Seite "Wiedergabelistenressourcen"](media/custom_slist.png)

Sie können auch die zuvor erstellte SharePoint-Seite hinzufügen oder eine von Grund auf in der Oberfläche erstellen.

1. Klicken Sie **im** Dialogfeld Wiedergabelistenressourcen auf die Option Neues Objekt.
1. Geben Sie Ihrem Objekt einen **Titel**. Nach der Eingabe werden zusätzliche Optionen angezeigt.
![Formular, in dem Sie Den Titel und weitere Details eingeben.](media/custom_newpage.png)
1. Sie können nun eine neue Objektseite in SharePoint Online erstellen oder die URL einer vorhandenen Seite eingeben, um sie ihrer benutzerdefinierten Wiedergabeliste hinzuzufügen. 
1. Die Felder **Kategorie,** **Unterkategorie** und Technologie werden basierend auf Ihrer vorherigen Auswahl für diese Wiedergabeliste vorab ausgefüllt. 
1. Treffen Sie die entsprechende Auswahl für Ebene und Zielgruppe für diese einzelne Ressource.  
1. Klicken **Sie auf Asset speichern,** um es der benutzerdefinierten Wiedergabeliste hinzuzufügen.
1. Wiederholen Sie diese Schritte, indem Sie entweder einzelne Seiten suchen oder hinzufügen, bis Ihre Wiedergabeliste abgeschlossen ist. 
1. Klicken **Sie auf Wiedergabeliste schließen,** um zu speichern

Ihre Wiedergabeliste mit diesen Inhalten steht jetzt überall dort zur Verfügung, wo Sie das Custom Learning-Webpart installiert/eingebettet haben. 

> [!NOTE]
> Wenn Sie einen Fehler machen, nachdem Sie die Wiedergabeliste geschlossen haben, können Sie sie aus der Kategorie löschen, indem Sie auf das X neben dem Wiedergabelistennamen klicken.  

#### <a name="things-to-think-about"></a>Dinge, über die Sie nachdenken sollten

Benutzerdefinierte Wiedergabelisten können verwendet werden, um Endbenutzern bei einer Vielzahl von Aufgaben zu helfen.  Verfügen Sie über ein Anforderungsformular für Zeits off?  Ein Formular zum Anfordern von Hardwaregeräten?  Alle vorhandenen Schulungsressourcen können in die Erfahrung programmiert werden.  

## <a name="share-playlists"></a>Freigeben von Wiedergabelisten

1. Navigieren zu einer beliebigen Wiedergabeliste innerhalb des Webparts oder der Websiteerfahrung
1. In der linken oberen Ecke werden drei Symbole angezeigt.
1. Klicken Sie auf das Symbol, das einen Link darstellt.
1. Kopieren Sie die URL in den ![ Wiedergabelistenbildschirm, in dem Sie neben der URL auf Kopieren klicken.](media/share.png)
Diese URL kann nun in Ihre Websitenavigation eingefügt oder in anderer Kommunikation verwendet werden, um Ihre Mitarbeiter direkt zu dieser Wiedergabeliste zu wechseln. 

### <a name="next-steps---drive-adoption"></a>Nächste Schritte – [Einführung des Laufwerks](driveadoption.md)
