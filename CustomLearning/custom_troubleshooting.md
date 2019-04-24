---
author: pkrebs
ms.author: pkrebs
title: Problembehandlung bei benutzerdefiniertem lernen
ms.date: 02/10/2019
description: Informationen zur Behandlung von benutzerdefiniertem lernen
ms.openlocfilehash: 7cbd049d4794d14f9e8cc26fd0db5f444812d688
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055090"
---
# <a name="troubleshoot-custom-learning"></a>Problembehandlung bei benutzerdefiniertem lernen

Hier finden Sie Tipps zur Problembehandlung bei Problemen, die mit benutzerdefiniertem lernen für Office 365 oder dem SharePoint Online-bereitstellen Dienst auftreten können.

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>So erfahren Sie, ob Sie über MandantenAdministrator Berechtigungen verfügen

Melden Sie sich beim SharePoint Online-proarbeits Dienst und der benutzerdefinierten Schulung an. Wenn Sie Probleme mit der Anmeldung beim SharePoint Online-bereit stellungs Dienst haben, stellen Sie sicher, dass Ihnen die globale Administratorrolle zugewiesen wurde. Die benutzerdefinierte Lernlösung erfordert MandantenAdministrator Berechtigungen, auch bekannt als globale Administrator Rolle von Office 365. Hier erfahren Sie, wie Sie feststellen, ob Ihnen die globale Administrator Rolle zugewiesen wurde.

1.  Melden Sie sich bei Office.com an.
2.  Klicken Sie auf **Admin**
3.  Wählen Sie unter **Benutzer**die Option **aktive Benutzer** aus.
4.  Suchen nach Ihrem Namen
5.  Klicken Sie in den Suchergebnissen auf Ihren Namen. Sie sollten den globalen Administrator für ihre Rolle sehen.

![CG-globaladminrole. png](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>Wenn Sie nicht über die globale Administratorrolle verfügen
- Suchen Sie nach einem globalen Administrator in Ihrer Organisation, und lassen Sie diese Person sich beim Dienst anmelden, oder weisen Sie Ihnen die globale Administratorrolle zu.

## <a name="tenant-app-catalog-troubleshooting"></a>Problembehandlung beim Mandanten-App-Katalog
Für benutzerdefiniertes lernen muss ein App-Katalog im Zielmandanten eingerichtet werden. Das Erstellen eines App-Katalogs erfordert globale Administrator Berechtigungen. Hier finden Sie die Schritte zur Problembehandlung für häufige Probleme mit dem App-Katalog:

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>So erfahren Sie, ob Sie einen Mandanten-App-Katalog haben 
Stellen Sie sicher, dass Sie über globale Administratorberechtigungen verfügen. Lesen Sie die Schritte für MandantenAdministrator-Berechtigungen oben.

1. klicken sie in Office 365 auf **administrator**, klicken sie auf den pfeil >, klicken sie auf **alle** > **admin center** > **sharepoint**anzeigen.
2. Klicken Sie auf **klassische admin SharePoint Center** > **apps** > -**App-Katalog**.
3. Unter **apps**sollte eine Kachel mit dem Titel Distribute **apps for SharePoint**angezeigt werden. Wenn die Kachel angezeigt wird, haben Sie einen Mandanten-App-Katalog. Weitere Informationen finden Sie unter **How to sicher your are a Site colllection...** section below. Wenn die Kachel nicht angezeigt wird, müssen Sie einen Mandanten-App-Katalog für Ihren Mandanten erstellen. Weitere Informationen finden Sie im Abschnitt **So erstellen Sie einen Mandanten-App-Katalog** .

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>So stellen Sie sicher, dass Sie ein WebsitesammlungsBesitzer im Mandanten-App-Katalog sind 
Um benutzerdefiniertes lernen für Office 365 zu stellen, müssen Sie ein WebsitesammlungsBesitzer im Mandanten-App-Katalog sein. Hier erfahren Sie, wie Sie feststellen, ob Sie ein Besitzer sind.

1. klicken sie in Office 365 auf **administrator**, klicken sie auf den pfeil >, klicken sie auf **alle** > **admin center** > **sharepoint**anzeigen.
2. Klicken Sie auf **klassische admin SharePoint Center**, und wählen Sie dann den **App-Katalog**aus.
3. Wählen Sie **Besitzer**aus, und stellen Sie sicher, dass Sie ein Websitesammlungsbesitzer sind. Es sollte ungefähr wie folgt aussehen.
 
![CG-sitecollectionowner. png](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>Erstellen eines Mandanten-App-Katalogs, falls nicht vorhanden 
1. Melden Sie sich bei Office 365 mit Ihrem SharePoint Online-Administratorkonto an.
2. Klicken Sie auf **Administrator**.
3. Klicken Sie unter **Admin Centers**auf **SharePoint**. 
4. Klicken Sie auf **apps** > -**App-Katalog**.
5. Klicken Sie auf **neue APP-katalogwebsite erstellen**, und klicken Sie dann auf **OK**. 
6.  Geben Sie die Informationen für den App-Katalog ein. Möglicherweise möchten Sie mehrere Administratoren einbeziehen. Nachfolgend sehen Sie ein Beispiel.  

![CG-appcatalogfinish. png](media/cg-appcatalogfinish.png)

7.  Fertig! Sie sind fertig. Bevor Sie jedoch zur Bereitstellung von benutzerdefiniertem lernen wechseln, müssen Sie mindestens 30 Minuten warten, um sicherzustellen, dass die Erstellung des App-Katalogs abgeschlossen ist. 

> [!IMPORTANT]
> Warten Sie nach dem Erstellen des Mandanten-App-Katalogs mindestens 30 Minuten, bevor Sie benutzerdefiniertes lernen einrichten. Dadurch wird sichergestellt, dass der APP-Katalog Bereitstellung in SharePoint abgeschlossen ist. 