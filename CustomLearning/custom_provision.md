---
author: pkrebs
ms.author: pkrebs
title: Bereitstellungswebsite für Microsoft 365-Lern Pfade
ms.date: 02/10/2019
description: Stellen der Website "Microsoft 365 Learning Pfads" über den SharePoint-Bereitstellungsdienst
ms.openlocfilehash: 7bffd8ae68099e8def1fa7a8b8620d95b4b65740
ms.sourcegitcommit: f4c2b6ef531d2d820c3d97871e187d0a2220d8f4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/04/2019
ms.locfileid: "37956677"
---
# <a name="provision-microsoft-365-learning-pathways"></a>Stellen von Microsoft 365-Lernpfaden

Mit dem SharePoint Online-Bereitstellung-Dienst kann ein Office 365-Mandanten Administrator den Bereitstellung-Prozess mit wenigen einfachen Klicks starten. Der Bereitstellungsdienst ist die empfohlene Vorgehensweise für Lern Pfade. Es ist schnell, einfach und dauert nur ein paar Minuten, um den Prozess zu starten. Stellen Sie jedoch sicher, dass Sie die Voraussetzungen für die Bereitstellung erfüllt haben, bevor Sie mit dem Bereitstellung-Dienst beginnen.

> [!IMPORTANT]
> Ab 5/21/2019 sind Microsoft 365-Lern Pfade der neue Name für die Lösung, die früher als benutzerdefiniertes lernen für Office 365 bezeichnet wurde. Wenn Sie bereits benutzerdefiniertes lernen für Office 365 oder eine frühere Version von Microsoft 365-Lernpfaden in Ihrer Organisation eingerichtet haben und die Lösung aktualisieren möchten, befolgen Sie die Anweisungen zum Aktualisieren der Lösung in den [Lernabschnitten zu Microsoft 365. Readme](https://github.com/pnp/custom-learning-office-365). Wenn Sie Microsoft 365-Lern Pfade erstmalig zur Verfügung stellen, finden Sie weitere Informationen in der Microsoft 365-Lern Pfad Dokumentation unter [Provision Microsoft 365 Learning]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision) Pfads.  

## <a name="prerequisites"></a>Voraussetzungen
 
Um Microsoft 365-Lernpfade mit dem Dienst für die Einrichtung erfolgreich einzurichten, muss die Person, die die Provision ausführt, die folgenden Voraussetzungen erfüllen: 
 
- Die Person, die Lernpfade ausstellt, muss ein Mandanten Administrator des Mandanten sein, in dem Lern Pfade eingerichtet werden.  
- Ein Mandanten-App-Katalog muss in der apps-Option des SharePoint Admin Center verfügbar sein. Wenn Ihre Organisation nicht über einen SharePoint-Mandanten-App-Katalog verfügt, lesen Sie in der [SharePoint Online Dokumentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) nach, um eine zu erstellen.  
- Die Person, die Lern Pfade anstellt, muss ein Websitesammlungsbesitzer des Mandanten-App-Katalogs sein. Wenn die Person, die Lern Pfade anbietet, kein Websitesammlungsbesitzer des App-Katalogs ist, [führen Sie diese Anweisungen](addappadmin.md) aus, und fahren Sie fort. 

### <a name="to-provision-learning-pathways"></a>So stellen Sie Lern Pfade zur Verfügung

1. Wechseln Sie zur [Seite Microsoft 365 Learning Pfads Solution](https://provisioning.sharepointpnp.com/details/3df8bd55-b872-4c9d-88e3-6b2f05344239).
2. Klicken Sie auf **zu Ihrem Mandanten hinzufügen**. Wenn Sie nicht bei Ihrem Mandanten angemeldet sind, werden Sie vom Dienst für die Verwaltung aufgefordert, Ihre Mandanten-Administratoranmeldeinformationen einzugeben. 
3. Wählen Sie im Dialogfeld angeforderte Berechtigungen die Option **Zustimmung im Namen Ihrer Organisation** aus, und wählen Sie dann **annehmen**aus.

Für den Bereitstellungsdienst sind diese Berechtigungen erforderlich, um den Mandanten-App-Katalog zu erstellen, die Anwendung in den Mandanten-App-Katalog zu installieren und die Websitevorlage zur Verfügung zu stellen. Es gibt keine allgemeinen Auswirkungen auf ihren Mandanten, und diese Berechtigungen werden explizit für den Zweck der Lösungsinstallation verwendet. Sie müssen diese Berechtigungen akzeptieren, um mit der Installation fortzufahren.

4. Füllen Sie die Felder auf der Seite Informationen zur Datenverarbeitung entsprechend für Ihre Installation aus. Geben Sie mindestens die e-Mail-Adresse ein, unter der Sie Benachrichtigungen über den Bereitstellung-Prozess und die Ziel-URL für die Bereitstellung Ihrer Website erhalten möchten.  
> [!NOTE]
> Stellen Sie die Ziel-URL für Ihre Website so freundlich wie "/Sites/MyTraining" oder "/Teams/LearnMicrosoft365" für Ihre Mitarbeiter dar.

![inst_options. png](media/inst_options.png)

6. Klicken Sie auf bereit **Stellung** , wenn Sie Lern Pfade in Ihrer Mandanten Umgebung installieren möchten.  Der bereit stellungsprozess dauert bis zu 15 Minuten. Wenn die Website für den Zugriff verfügbar ist, werden Sie per e-Mail benachrichtigt (an die e-Mail-Adresse der Benachrichtigung, die Sie auf der Seite für die Einrichtung eingegeben haben). 

> [!IMPORTANT]
> Der mandantenadministrator, der die Website für Lern Pfade bereitstellt, muss zur Website wechseln und dann **CustomLearningAdmin. aspx** öffnen, um die Administrator Eigenschaften für Lern Pfade zu initialisieren. Zu diesem Zeitpunkt sollte der mandantenadministrator dem Standort auch Besitzer zuweisen. 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Überprüfen des Erfolgs der Vorstellung und Initialisieren der CustomConfig-Liste

Wenn die proprovisionierung abgeschlossen ist, erhält der mandantenadministrator, der die Website vorsieht, eine e-Mail vom PnP-Dienst für die Zustellung. Die e-Mail enthält einen Link zu der Website. An dieser Stelle sollte der mandantenadministrator die Website über den in der e-Mail angegebenen Link aufrufen und die Website für die erste Verwendung einrichten:

- Navigieren Sie in das Verzeichnis `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`. Beim Öffnen von **CustomLearningAdmin. aspx** wird das **CustomConfig** -Listenelement initialisiert, das Lern Pfade für die erste Verwendung einrichtet. Sie sollten eine Seite sehen, die wie folgt aussieht:

![CG-adminapppage. png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Hinzufügen von Besitzern zur Website
Als mandantenadministrator ist es unwahrscheinlich, dass Sie die Person anpassen, die die Website anpasst, sodass Sie der Website einige Besitzer zuweisen müssen. Besitzer verfügen über Administratorrechte für die Website, damit Sie Website Seiten ändern und die Website neu Branding können. Außerdem können Sie Inhalte, die über das Lern Pfade-Webpart übermittelt werden, ausblenden und anzeigen. Darüber hinaus haben Sie die Möglichkeit, benutzerdefinierte Wiedergabelisten zu erstellen und Sie benutzerdefinierten Unterkategorien zuzuweisen.  

1. Klicken Sie im Menü SharePoint- **Einstellungen** auf **Websiteberechtigungen**.
2. Klicken Sie auf **Erweiterte Berechtigungseinstellungen**.
3. Klicken Sie auf **Microsoft 365 Lern Pfad Besitzer**.
4. Klicken Sie auf **neu** > **Hinzufügen von Benutzern zu dieser Gruppe**, und fügen Sie dann die Personen hinzu, die Besitzer sein sollen. 
5. Fügen Sie einen Link zum [Durchsuchen der Website](custom_exploresite.md) in der Freigabenachricht hinzu, und klicken Sie dann auf **Freigeben**.

### <a name="next-steps"></a>Nächste Schritte
- Erkunden Sie die in der Website und im Webpart bereitgestellten [Standardinhalte](custom_exploresite.md) .
