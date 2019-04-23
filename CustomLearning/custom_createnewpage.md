---
author: pkrebs
ms.author: pkrebs
title: Erstellen von SharePoint-Seiten für Wiedergabelisten
ms.date: 02/10/2019
description: Erstellen von SharePoint-Seiten für Wiedergabelisten
ms.openlocfilehash: c2de66a0746260e8f6539656ad70052b209c54ba
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055495"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a>Erstellen von SharePoint-Seiten für benutzerdefinierte Wiedergabelisten

Eine der einzigartigen Features von benutzerdefiniertem lernen ist die Möglichkeit, Wiedergabelisten zu erstellen, die aus Objekten aus Microsoft und aus von Ihnen erstellten SharePoint-Objekten zusammengestellt werden. In diesem Beispiel erstellen wir eine SharePoint-Seite vor dem Erstellen einer Wiedergabeliste. Die Möglichkeit, Wiedergabelisten von SharePoint-Seiten zu erstellen, bietet eine Vielzahl von Möglichkeiten zum Erstellen von Seiten mithilfe der Webparts, die von Microsoft oder Ihrer Organisation zur Verfügung stehen. Eine Wiedergabeliste kann beispielsweise eine SharePoint-Seite mit eingebetteten Videos von YouTube oder ein aus Office 365-Formularen erstelltes Formular oder einen eingebetteten Power BI-Bericht aufweisen. In diesem Beispiel wird gezeigt, wie Sie eine Seite mit dem Webpart "embed" und dem Webpart "Text" erstellen.  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a>Erstellen einer SharePoint-Seite für eine benutzerdefinierte Wiedergabeliste

1. Klicken Sie auf das SharePoint **Gear** -Symbol, und klicken Sie dann auf **Seite hinzufügen**.
2. Klicken Sie Links auf der Seite auf **neuen Abschnitt hinzufügen (+)** , und klicken Sie dann auf **zwei Spalten** für das Abschnittslayout.
3. Klicken Sie in der linken Spalte auf +, und klicken Sie dann auf das Webpart **embed** . 
4. Klicken Sie in der rechten Spalte auf +, und klicken Sie dann auf das Webpart **Text** . Ihre Seite sollte wie folgt aussehen.

![CG-pagenewstart. png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a>Hinzufügen eines Videos und Texts von YouTube

1. Wechseln Sie in Ihrem Browser zu YouTube. Suchen Sie in diesem Beispiel nach "Was ist Office 365 – die besten Produktivitäts-apps von Microsoft".
2. Klicken Sie auf das Video, um es wiederzugeben, und klicken Sie dann mit der rechten Maustaste darauf. 
3. Klicken Sie auf **embed-Code kopieren**und dann zur SharePoint-Seite zurückkehren. 
4. Klicken Sie im **embed** -Webpart auf **embed-Code hinzufügen** , und fügen Sie dann den Code aus dem YouTube-Video hinzu.
5. Kehren Sie zur YouTube-Seite zurück **** , und kopieren Sie den Beschreibungstext für das Video. 
6. Kehren Sie zur Seite SharePoint zurück, wählen Sie das Webpart **Text** aus, und kopieren Sie dann den Text aus dem YouTube-Video.
7. Wählen Sie das Symbol **Webpart bearbeiten** im titelBereich der SharePoint-Seite aus, und nennen Sie dann die Seite "benutzerdefinierte Playlist-Einführung". 
8. Wählen Sie unter **Layout**die Option **Plain**aus, und schließen Sie dann den Bereich **Title Region** Properties. Die Seite sollte jetzt ungefähr wie folgt aussehen. 

![CG-pagenewfinish. png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a>Seite veröffentlichen

- Klicken Sie auf die Schaltfläche **veröffentlichen** . Jetzt können Sie diese SharePoint-Seite Ihrer benutzerdefinierten Wiedergabeliste hinzufügen. 