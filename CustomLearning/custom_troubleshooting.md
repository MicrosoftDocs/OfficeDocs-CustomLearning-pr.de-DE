---
author: pkrebs
ms.author: pkrebs
title: Problembehandlung bei Microsoft 365-Lernpfaden
ms.date: 02/10/2019
description: Informationen zur Problembehandlung für Microsoft 365-Lern Pfade
ms.openlocfilehash: de46b9c754dac36de230b36ec4a5542518a1dcd5
ms.sourcegitcommit: 1a111a49a0413a56a880e29109ba01b5e5f33d09
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/20/2019
ms.locfileid: "34247680"
---
# <a name="troubleshoot-microsoft-365-learning-pathways"></a>Problembehandlung bei Microsoft 365-Lernpfaden

Hier finden Sie Tipps zur Problembehandlung bei Problemen, die mit Microsoft 365-Lernpfaden oder dem SharePoint Online Bereitstellung-Dienst auftreten können.

## <a name="how-to-know-if-you-have-tenant-admin-permissions"></a>So erfahren Sie, ob Sie über mandantenadministrator Berechtigungen verfügen

Melden Sie sich beim SharePoint Online-Dienst für die Einrichtung und für die benutzerdefinierte Vorgehensweise für die Verwaltung von Mandanten Berechtigungen an. Wenn Sie mit dem SharePoint Online-Bereitstellung-Dienst Probleme mit der Anmeldung haben, stellen Sie sicher, dass Ihnen die globale Administratorrolle zugewiesen wurde. Für die benutzerdefinierte Lernlösung sind mandantenadministrator Berechtigungen erforderlich, die andernfalls als Office 365 globale Administrator Rolle bezeichnet werden. Hier erfahren Sie, wie Sie feststellen, ob Ihnen die globale Administrator Rolle zugewiesen wurde.

1.  Melden Sie sich bei Office.com an.
2.  Klicken Sie auf **Administrator**
3.  Wählen Sie unter **Benutzer**die Option **aktive Benutzer** aus.
4.  Suchen nach Ihrem Namen
5.  Klicken Sie in den Suchergebnissen auf Ihren Namen. Sie sollten den globalen Administrator für ihre Rolle sehen.

![CG-globaladminrole. png](media/cg-globaladminrole.png)

### <a name="if-you-dont-have-the-global-administrator-role"></a>Wenn Sie nicht über die globale Administratorrolle verfügen
- Suchen Sie einen globalen Administrator in Ihrer Organisation, und lassen Sie diese Person sich beim Dienst anmelden, oder weisen Sie Ihnen die globale Administratorrolle zu.

## <a name="tenant-app-catalog-troubleshooting"></a>Problembehandlung für den Mandanten-App-Katalog
Für benutzerdefiniertes lernen muss ein App-Katalog im Zielmandanten vorgesehen werden. Das Erstellen eines App-Katalogs erfordert globale Administrator Berechtigungen. Es folgen die Schritte zur Problembehandlung für häufige Probleme mit dem App-Katalog:

### <a name="how-to-know-if-you-have-a-tenant-app-catalog"></a>So erfahren Sie, ob Sie über einen Mandanten-App-Katalog verfügen 
Stellen Sie zunächst sicher, dass Sie über globale Administratorberechtigungen verfügen. Siehe die Schritte für Mandanten-Administratorberechtigungen oben.

1. Klicken Sie in Office 365 auf **Administrator**, klicken Sie auf den Pfeil > erweitern, und klicken Sie dann auf **alle** > **SharePoint**-**Verwaltungscenter** > anzeigen.
2. Klicken Sie auf **Classic admin SharePoint Center** > **apps** > -**App-Katalog**.
3. Unter **apps**sollte eine Kachel mit dem Titel Distribute **apps for SharePoint**angezeigt werden. Wenn die Kachel angezeigt wird, haben Sie einen Mandanten-App-Katalog. Weitere Informationen finden Sie im Abschnitt **How to sicher your are a Site colllection...** Wenn die Kachel nicht angezeigt wird, müssen Sie einen Mandanten-App-Katalog für Ihren Mandanten erstellen. Weitere Informationen finden Sie im Abschnitt **Erstellen eines Mandanten-App** -Katalogs weiter unten.

### <a name="how-to-ensure-you-are-a-site-collection-owner-on-the-tenant-app-catalog"></a>Vorgehensweise sicherstellen, dass Sie ein Websitesammlungsbesitzer im Mandanten-App-Katalog sind 
Um Microsoft 365-Lern Pfade zur Verfügung zu stellen, müssen Sie ein Websitesammlungsbesitzer im Mandanten-App-Katalog sein. Hier erfahren Sie, wie Sie feststellen können, ob Sie ein Besitzer sind.

1. Klicken Sie in Office 365 auf **Administrator**, klicken Sie auf den Pfeil > erweitern, und klicken Sie dann auf **alle** > **SharePoint**-**Verwaltungscenter** > anzeigen.
2. Klicken Sie auf **klassisches admin SharePoint Center**, und wählen Sie dann den **App-Katalog**aus.
3. Wählen Sie **Besitzer**aus, und stellen Sie sicher, dass Sie ein Websitesammlungsbesitzer sind. Es sollte in etwa wie folgt aussehen.
 
![CG-sitecollectionowner. png](media/cg-sitecollectionowner.png)

### <a name="how-to-create-a-tenant-app-catalog-if-one-doesnt-exists"></a>Vorgehensweise Erstellen eines Mandanten-App-Katalogs, falls nicht vorhanden 
1. Melden Sie sich bei Office 365 mit Ihrem SharePoint Online-Administratorkonto an.
2. Klicken Sie auf **Administrator**.
3. Klicken Sie unter **Admin Center**auf **SharePoint**. 
4. Klicken Sie auf **apps** > -**App-Katalog**.
5. Klicken Sie auf **neue APP-katalogwebsite erstellen**, und klicken Sie dann auf **OK**. 
6.  Geben Sie die Informationen für den App-Katalog ein. Möglicherweise möchten Sie mehr als einen Administrator einbeziehen. Im folgenden sehen Sie ein Beispiel.  

![CG-appcatalogfinish. png](media/cg-appcatalogfinish.png)

7.  Fertig! Sie sind fertig. Bevor Sie jedoch in das Bereitstellen von benutzerdefiniertem lernen umsetzen, müssen Sie mindestens 30 Minuten warten, um sicherzustellen, dass die APP-Katalogerstellung abgeschlossen ist. 

> [!IMPORTANT]
> Warten Sie mindestens 30 Minuten nach dem Erstellen des Mandanten-App-Katalogs, bevor Sie benutzerdefiniertes lernen einrichten. Dadurch wird sichergestellt, dass der App Catalog-bereit stellungsprozess in SharePoint abgeschlossen ist. 