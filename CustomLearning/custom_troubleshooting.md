---
author: pkrebs
ms.author: pkrebs
title: Problembehandlung für Microsoft 365 Lernpfade
ms.date: 02/10/2019
description: Informationen zur Problembehandlung von Microsoft 365-Lernpfaden
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 7190688d574042c8a1b8dfb67c8b246dfbf8c927
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000301"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a>Problembehandlung für Microsoft 365-Lernpfade

Hier finden Sie Tipps zur Problembehandlung bei Problemen, die mit Microsoft 365-Lernpfaden oder dem SharePoint Online-Bereitstellungsdienst auftreten können.

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>Wissen, ob Sie über Mandantenadministratorberechtigungen verfügen

Für die Anmeldung beim SharePoint Online-Bereitstellungsdienst und die Bereitstellung von Custom Learning sind Mandantenadministratorberechtigungen erforderlich. Wenn Anmeldeprobleme mit dem SharePoint Online-Bereitstellungsdienst auftreten, stellen Sie sicher, dass Ihnen die Rolle "Globaler Administrator" zugewiesen wurde. Für die Benutzerdefinierte Lernlösung sind Mandantenadministratorberechtigungen erforderlich, die auch als Office 365 Global Administrator-Rolle bezeichnet werden. Hier erfahren Sie, ob Ihnen die Rolle "Globaler Administrator" zugewiesen wurde.

1.  Melden Sie sich bei Office.com.
2.  Klicken Sie auf **Administrator**
3.  Wählen **Sie unter Benutzer** die Option Aktive Benutzer **aus.**
4.  Suchen nach Ihrem Namen
5.  Klicken Sie in den Suchergebnissen auf Ihren Namen. Sie sollten den globalen Administrator für Ihre Rolle sehen.
![Beispielseite, auf der Ihre Rolle zusammen mit Lizenzen, Gruppenmitgliedschaften und anderen Informationen aufgeführt ist.](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>Wenn Sie nicht über die Rolle "Globaler Administrator" verfügen
- Suchen Sie einen globalen Administrator in Ihrer Organisation, und lassen Sie diese Person beim Dienst anmelden, oder lassen Sie sie ihnen die Rolle "Globaler Administrator" zuweisen.

## <a name="tenant-app-catalog-troubleshooting"></a>Problembehandlung beim Mandanten-App-Katalog
Benutzerdefiniertes Lernen erfordert, dass ein App-Katalog im Ziel mandanten bereitgestellt wird. Für das Erstellen eines App-Katalogs sind globale Administratorberechtigungen erforderlich. Hier sind die Schritte zur Problembehandlung für häufige Probleme im App-Katalog:

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>Wissen, ob Sie über einen Mandanten-App-Katalog verfügen 
Stellen Sie zunächst sicher, dass Sie über globale Administratorberechtigungen verfügen. Weitere Informationen finden Sie in den oben aufgeführten Schritten für Mandantenadministratorberechtigungen.

1. Klicken Sie in Office 365 auf **Administrator,** klicken Sie auf den Pfeil > erweitern, klicken Sie auf **Alle**  >  **Admin Center**  >  **SharePoint anzeigen.**
2. Klicken **Sie auf Klassischer SharePoint Center-App-App-Katalog**  >    >  **für Administratoren.**
3. Unter **Apps** sollte eine Kachel mit dem Titel Verteilen von **Apps für SharePoint angezeigt werden.** Wenn die Kachel angezeigt wird, verfügen Sie über einen Mandanten-App-Katalog. Weitere Informationen **finden Sie unter How to ensure your are a Site Colllection...** weiter unten. Wenn die Kachel nicht angezeigt wird, müssen Sie einen Mandanten-App-Katalog für Ihren Mandanten erstellen. Weitere Informationen finden Sie im Abschnitt Erstellen **eines Mandanten-App-Katalogs** weiter unten.

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>So stellen Sie sicher, dass Sie Websitesammlungsbesitzer im Mandanten-App-Katalog sind 
Um Microsoft 365-Lernpfade bereitstellen zu können, müssen Sie websitesammlungsbesitzer im Mandanten-App-Katalog sein. Hier erfahren Sie, ob Sie ein Besitzer sind.

1. Klicken Sie in Office 365 auf **Administrator,** klicken Sie auf den Pfeil > erweitern, klicken Sie auf **Alle**  >  **Admin Center**  >  **SharePoint anzeigen.**
2. Klicken **Sie auf Klassisches Admin SharePoint Center,** und wählen Sie dann den **App-Katalog aus.**
3. Wählen **Sie Besitzer** aus, und stellen Sie dann sicher, dass Sie Websitesammlungsbesitzer sind. Es sollte etwa so aussehen.
![Seite "Administratoren verwalten".](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>Erstellen eines Mandanten-App-Katalogs, wenn er nicht vorhanden ist 
1. Melden Sie sich mit Ihrem SharePoint Online-Administratorkonto bei Office 365 an.
2. Klicken Sie auf **Administrator**.
3. Klicken **Sie unter Admin Center** auf **SharePoint**. 
4. Klicken Sie **auf**  >  **Apps-App-Katalog**.
5. Klicken **Sie auf Neue App-Katalogwebsite erstellen,** und klicken Sie dann auf **OK**. 
6.  Geben Sie die Informationen für den App-Katalog ein. Möglicherweise möchten Sie mehr als einen Administrator enthalten. Das folgende Beispiel zeigt ein Beispiel.  
![Formular zum Eingeben von Informationen für einen neuen App-Katalog.](media/cg-appcatalogfinish.png)

7.  Fertig! Sie sind fertig. Bevor Sie jedoch zur Bereitstellung von Custom Learning wechseln, müssen Sie mindestens 30 Minuten warten, um sicherzustellen, dass die Erstellung des App-Katalogs abgeschlossen ist. 

> [!IMPORTANT]
> Warten Sie mindestens 30 Minuten nach dem Erstellen des Mandanten-App-Katalogs, bevor Sie benutzerdefiniertes Lernen bereitstellen. Dadurch wird sichergestellt, dass der Bereitstellungsprozess für den App-Katalog in SharePoint abgeschlossen ist. 