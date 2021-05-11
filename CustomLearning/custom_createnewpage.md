---
author: pkrebs
ms.author: pkrebs
title: Erstellen SharePoint Seiten für Wiedergabelisten
ms.date: 02/10/2019
description: Erstellen SharePoint Seiten für Wiedergabelisten
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
ms.openlocfilehash: ce4a204b3072469840b6f3fa8f93d9e78833b181
ms.sourcegitcommit: 956ab22dd8ce23ee1779f1a01d34b434243c3cb1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/11/2021
ms.locfileid: "52310659"
---
# <a name="create-sharepoint-pages-for-custom-playlists"></a>Erstellen SharePoint Seiten für benutzerdefinierte Wiedergabelisten

Eines der einzigartigen Features von Lernpfaden ist die Möglichkeit, Wiedergabelisten zu erstellen, die aus Ressourcen von Microsoft und aus SharePoint erstellt werden. In diesem Beispiel erstellen wir eine SharePoint vor dem Erstellen einer Wiedergabeliste. Die Möglichkeit, Wiedergabelisten aus SharePoint Seiten zu erstellen, bietet eine Vielzahl von Möglichkeiten zum Erstellen von Seiten mithilfe der von Microsoft oder Ihrer Organisation verfügbaren Webparts. Eine Wiedergabeliste kann z. B. eine SharePoint mit eingebetteten Videos von YouTube oder ein formular erstellt aus Office 365 Forms oder einen eingebetteten Power BI enthalten. In diesem Beispiel wird gezeigt, wie Sie eine Seite mit dem Embed-Web part und dem Text-Web part erstellen.  

## <a name="create-a-sharepoint-page-for-a-custom-playlist"></a>Erstellen einer SharePoint für eine benutzerdefinierte Wiedergabeliste

1. Klicken Sie auf SharePoint **Zahnradsymbol,** und klicken Sie dann **auf Seite hinzufügen**.
2. Klicken Sie auf der linken Seite der Seite auf Neuen Abschnitt **hinzufügen (+),** und klicken Sie dann auf **Zwei** Spalten für das Abschnittslayout.
3. Klicken Sie in der linken Spalte auf + , und klicken Sie dann auf web part **einbetten.** 
4. Klicken Sie in der rechten Spalte auf  +, und klicken Sie dann auf das Textwebteil. Ihre Seite sollte wie dies aussehen.

![cg-pagenewstart.png](media/cg-pagenewstart.png)

### <a name="add-a-video-and-text-from-youtube"></a>Hinzufügen eines Videos und Texts aus YouTube

1. Wechseln Sie in Ihrem Browser zu YouTube. Suchen Sie in diesem Beispiel nach "Was ist Office 365 – Microsofts beste Produktivitäts-Apps".
2. Klicken Sie auf das Video, um es wieder zu spielen, halten Sie es an, und klicken Sie dann mit der rechten Maustaste darauf. 
3. Klicken **Sie auf Einbettungscode** kopieren, und kehren Sie dann zur Seite SharePoint zurück. 
4. Klicken **Sie im** **Web** part Embed auf Einbettungscode hinzufügen, und fügen Sie dann den Code aus dem YouTube-Video hinzu.
5. Kehren Sie zur YouTube-Seite zurück, und kopieren Sie **den Beschreibungstext** für das Video. 
6. Kehren Sie zur seite SharePoint,  wählen Sie das Text-Webteil aus, und kopieren Sie dann den Text aus dem YouTube-Video.
7. Wählen Sie **das Symbol Webteil** bearbeiten im Bereich Titel der Seite SharePoint aus, und nennen Sie dann die Seite "Benutzerdefinierte Wiedergabelisteneinführung". 
8. Wählen **Sie unter Layout** die Option **Nur** aus, und schließen Sie dann den **Eigenschaftenbereich Titelbereich.** Die Seite sollte nun etwa wie folgt aussehen. 

![cg-pagenewfinish.png](media/cg-pagenewfinish.png)

### <a name="publish-the-page"></a>Veröffentlichen der Seite

- Wählen Sie die **Schaltfläche Veröffentlichen** aus. Jetzt können Sie diese Seite SharePoint ihrer benutzerdefinierten Wiedergabeliste hinzufügen. 