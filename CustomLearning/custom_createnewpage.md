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
# <a name="create-sharepoint-pages-for-custom-playlists"></a>Erstellen von SharePoint-Seiten für benutzerdefinierte Wiedergabelisten

Eines der einzigartigen Features von Lernpfaden ist die Möglichkeit, Wiedergabelisten zu erstellen, die aus Ressourcen von Microsoft und aus erstellten SharePoint-Ressourcen zusammengestellt werden. In diesem Beispiel erstellen wir vor dem Erstellen einer Wiedergabeliste eine SharePoint-Seite. Die Möglichkeit, Wiedergabelisten aus SharePoint-Seiten zu erstellen, bietet eine Vielzahl von Möglichkeiten zum Erstellen von Seiten mithilfe der von Microsoft oder Ihrer Organisation verfügbaren Webparts. Eine Wiedergabeliste kann z. B. eine SharePoint-Seite mit eingebetteten Videos aus YouTube oder ein aus Office 365 Forms erstelltes Formular oder einen eingebetteten Power BI-Bericht enthalten. In diesem Beispiel wird gezeigt, wie Sie eine Seite mit dem Embed-Web part und dem Text-Web part erstellen.  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a>Erstellen einer SharePoint-Seite für eine benutzerdefinierte Wiedergabeliste

1. Klicken Sie auf das Symbol SharePoint **Gear,** und klicken Sie dann **auf Seite hinzufügen.**
2. Klicken Sie auf der linken Seite der Seite auf Neuen Abschnitt **hinzufügen (+),** und klicken Sie dann auf **Zwei** Spalten für das Abschnittslayout.
3. Klicken Sie in der linken Spalte auf + , und klicken Sie dann auf web part **einbetten.** 
4. Klicken Sie in der rechten Spalte auf  +, und klicken Sie dann auf das Textwebteil. Ihre Seite sollte wie dies aussehen.

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a>Hinzufügen eines Videos und Texts aus YouTube

1. Wechseln Sie in Ihrem Browser zu YouTube. Suchen Sie in diesem Beispiel nach "Was ist Office 365 – Die besten Produktivitäts-Apps von Microsoft".
2. Klicken Sie auf das Video, um es wieder zu spielen, halten Sie es an, und klicken Sie dann mit der rechten Maustaste darauf. 
3. Klicken **Sie auf Einbettungscode** kopieren, und kehren Sie dann zur SharePoint-Seite zurück. 
4. Klicken **Sie im** **Web** part Embed auf Einbettungscode hinzufügen, und fügen Sie dann den Code aus dem YouTube-Video hinzu.
5. Kehren Sie zur YouTube-Seite zurück, und kopieren Sie **den Beschreibungstext** für das Video. 
6. Kehren Sie zur Seite SharePoint zurück, wählen Sie das **Textwebteil** aus, und kopieren Sie dann den Text aus dem YouTube-Video.
7. Wählen Sie **das Symbol Webteil** bearbeiten im Bereich Titel der SharePoint-Seite aus, und nennen Sie dann die Seite "Benutzerdefinierte Wiedergabelisteneinführung". 
8. Wählen **Sie unter Layout** die Option **Nur** aus, und schließen Sie dann den **Eigenschaftenbereich Titelbereich.** Die Seite sollte nun etwa wie folgt aussehen. 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a>Veröffentlichen der Seite

- Wählen Sie die **Schaltfläche Veröffentlichen** aus. Jetzt können Sie diese SharePoint-Seite ihrer benutzerdefinierten Wiedergabeliste hinzufügen. 