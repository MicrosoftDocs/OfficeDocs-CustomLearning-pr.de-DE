---
author: karuanag
ms.author: karuanag
title: Installieren der benutzerdefinierten Learning Solution-Webpart
ms.date: 02/10/2019
description: Installationsanweisungen für die benutzerdefinierte Lernlösung Webpart
ms.openlocfilehash: 53229e5b1b8175b06d888091963d1a9f2f0bd361
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/25/2019
ms.locfileid: "29989686"
---
# <a name="installing-the-custom-learning-solution-webpart"></a>Installieren der benutzerdefinierten Learning Solution-Webpart

## <a name="prerequisites-for-a-tenant-wide-installation"></a>VoraussetZungen für eine Mandantenweite Installation

- Um das benutzerdefinierte Lern Webpart für Ihren gesamten Mandanten zu installieren, benötigen Sie Office 365-Administratorberechtigungen.  Wenn Sie nicht über diese Berechtigungen verfügen, können Sie entweder mit Ihrem Office 365-Administrator zusammenarbeiten oder das Webpart für eine einzelne Websitesammlung installieren.
- Sie oder Ihr Office 365-Administrator müssen einen Mandanten weiten [App-Katalog](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant) oder einen [Website Sammlungs-App-Katalog](https://docs.microsoft.com/en-us/sharepoint/dev/general-development/site-collection-app-catalog)einrichten und konfigurieren, um den Webpart zu empfangen.]
- Wir unterstützen nur SharePoint Online. Das Webpart ist nicht für die Installation in einer beliebigen Version von SharePoint unterstützt.

## <a name="add-the-custom-learning-webpart-to-your-tenant"></a>Hinzufügen des benutzerdefinierten Learning-Webpart zu Ihrem Mandanten 

1. Laden Sie das benutzerdefinierte Lern Webpart herunter, und speichern Sie es auf Ihrem lokalen Laufwerk.  Diese Datei heißt "MS-Custom-Learning. sppkg".  Ändern Sie nicht den Namen oder das Suffix der Datei. 
2. Navigieren Sie zum [Office 365-Verwaltungsportal](https://admin.microsoft.com/AdminPortal/Home#/homepage) für Ihren Mandanten.
3. Wählen Sie im linken Navigationsbereich Admin Center, SharePoint aus. Sie wird in einer neuen Registerkarte geöffnet. Wählen Sie im SharePoint Admin Center apps, App-Katalog, Apps für SharePoint 
4. Wählen Sie Webpart Hochladen aus, und wählen Sie die Datei "MS-Custom-Learning. sppkg" aus, die Sie heruntergeladen haben.
5. Bei dieser Mandanten weiten Installation aktivieren Sie das Kontrollkästchen neben "Diese Lösung für alle verfügbar machen in der Organisation".  
 
> [!NOTE]
> Sobald das Webpart installiert ist, finden Sie es in Ihrem Webpart-Katalog in SharePoint Online.  **In der Galerie heißt das Webpart "Microsoft Learning"** .

![Bereitstelleneiner Lösung](media/trustapp_sm.png)


## <a name="add-the-microsoft-learning-webpart-to-a-sharepoint-online-page"></a>Hinzufügen des Microsoft Learning-Webpart zu einer SharePoint Online-Seite

Nachdem benutzerdefiniertes lernen in Ihrem Mandanten installiert wurde, können Sie das Webpart einer SharePoint-Seite hinzufügen. Wenn Sie Office 365 und Windows 10 trainieren, steht Ihre Website zur Verfügung.

1. Hinzufügen des benutzerdefinierten Learning-Webpart in einem Spaltenlayout mit voller Breite:

![SharePoint-Seiten Layout](media/clo365fullcolumnwidth.png)

2. Wählen Sie auf der Seite SharePoint die Option Abschnitt hinzufügen aus, und wählen Sie dann Spalte vollständiger Breite aus.  Die folgende Meldung wird angezeigt:

![AddWebpart](media/clo365addfullwidthwebpart.png)

3. Wählen Sie Microsoft Learning aus.  Es sollte jetzt Folgendes angezeigt werden: 

![Benutzerdefiniertes Learning-Webpart](media/clo365addwebpart.png)

 Sie können nun auf die Kacheln klicken, um die in der Lösung enthaltenen Standardinhalte zu erkunden.  

### <a name="next-steps"></a>Weitere Schritte
- Erkunden Sie die im Webpart enthaltenen [Standardinhalte](webpartcontent.md) .
- [Passen](customization.md) Sie die Schulungsumgebung für Ihre Organisation an.
- Führen Sie die [Einführung](driveadoption.md) ihrer Schulungslösung aus.

