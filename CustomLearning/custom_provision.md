---
author: pkrebs
ms.author: pkrebs
title: Bereitstellungswebsite für Microsoft 365-Lern Pfade
ms.date: 02/10/2019
description: Stellen der Website "Microsoft 365 Learning Pfads" über den SharePoint-Bereitstellungsdienst
ms.openlocfilehash: e48052a395a8669ef684110a1c93409f5859a1d2
ms.sourcegitcommit: 0077704d7edcc26eda76900115716fc5b7b1c518
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/21/2019
ms.locfileid: "34334743"
---
# <a name="provision-microsoft-365-learning-pathways"></a>Stellen von Microsoft 365-Lernpfaden

Mit dem SharePoint Online-Bereitstellung-Dienst kann ein Office 365-Mandanten Administrator den Bereitstellung-Prozess mit wenigen einfachen Klicks starten. Der Bereitstellungsdienst ist die empfohlene Vorgehensweise für Lern Pfade. Es ist schnell, einfach und dauert nur ein paar Minuten, um den Prozess zu starten. Stellen Sie jedoch sicher, dass Sie die Voraussetzungen für die Bereitstellung erfüllt haben, bevor Sie mit dem Bereitstellung-Dienst beginnen.

> [!IMPORTANT]
> Ab 5/21/2019 sind Microsoft 365-Lern Pfade der neue Name für die Lösung, die früher als benutzerdefiniertes lernen für Office 365 bezeichnet wurde. Wenn Sie bereits benutzerdefiniertes lernen für Office 365 in Ihrer Organisation eingerichtet haben und die Lösung aktualisieren möchten, befolgen Sie die Anweisungen "Aktualisieren der Lösung" in der [Readme-Datei zu Microsoft 365 Learning](https://github.com/pnp/custom-learning-office-365)-Pfaden. Wenn Sie Microsoft 365-Lern Pfade erstmalig zur Verfügung stellen, finden Sie weitere Informationen in der Microsoft 365-Lern Pfad Dokumentation unter [Provision Microsoft 365 Learning]( https://docs.microsoft.com/en-us/office365/customlearning/custom_provision) Pfads.  

## <a name="prerequisites"></a>Voraussetzungen
 
Um Microsoft 365-Lernpfade mit dem Dienst für die Einrichtung erfolgreich einzurichten, muss die Person, die die Provision ausführt, die folgenden Voraussetzungen erfüllen: 
 
- Die Person, die Lernpfade ausstellt, muss ein Mandanten Administrator des Mandanten sein, in dem Lern Pfade eingerichtet werden.  
- Ein Mandanten-App-Katalog muss in der apps-Option des SharePoint Admin Center verfügbar sein. Wenn Ihre Organisation nicht über einen SharePoint-Mandanten-App-Katalog verfügt, lesen Sie in der [SharePoint Online Dokumentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) nach, um eine zu erstellen.  
- Die Person, die Lern Pfade anstellt, muss ein Websitesammlungsbesitzer des Mandanten-App-Katalogs sein. Wenn die Person, die Lern Pfade anbietet, kein Websitesammlungsbesitzer des App-Katalogs ist, [führen Sie diese Anweisungen](addappadmin.md) aus, und fahren Sie fort. 

### <a name="to-provision-learning-pathways"></a>So stellen Sie Lern Pfade zur Verfügung

1. Wechseln Sie http://provisioning.sharepointpnp.com zu, und **melden** Sie sich von der oberen rechten Ecke der Startseite aus an.  Melden Sie sich mit den Anmeldeinformationen für den Zielmandanten an, in dem Sie die Websitevorlage installieren möchten.

![pnphome. png](media/inst_signin.png)

2. Löschen Sie die **Zustimmung im Namen Ihrer Organisation** , und wählen Sie **annehmen**aus.

![in](media/inst_perms.png)

Für den Bereitstellungsdienst sind diese Berechtigungen erforderlich, um den Mandanten-App-Katalog zu erstellen, die Anwendung in den Mandanten-App-Katalog zu installieren und die Websitevorlage zur Verfügung zu stellen. Es gibt keine allgemeinen Auswirkungen auf ihren Mandanten, und diese Berechtigungen werden explizit für den Zweck der Lösungsinstallation verwendet. Sie müssen diese Berechtigungen akzeptieren, um mit der Installation fortzufahren.

3. Scrollen Sie auf der Seite nach unten, wählen Sie die Registerkarte **Lösungen** aus, und wählen Sie dann **Lern Pfade für Office 365**aus. 

![in](media/inst_select.png)

4. Wählen Sie **zu Ihrem Mandanten hinzufügen**

![inst_select. png](media/inst_add.png)

5. Füllen Sie die Felder auf der Seite Informationen zur Datenverarbeitung entsprechend für Ihre Installation aus. Geben Sie mindestens die e-Mail-Adresse ein, unter der Sie Benachrichtigungen über den Bereitstellung-Prozess und die Ziel-URL für die Bereitstellung Ihrer Website erhalten möchten.  
> [!NOTE]
> Stellen Sie die Ziel-URL für Ihre Website so freundlich wie "/Sites/MyTraining" oder "/Teams/LearnMicrosoft365" für Ihre Mitarbeiter dar.

![inst_options. png](media/inst_options.png)

6. Wählen Sie **bereit** stellen aus, wenn Lern Pfade in Ihrer Mandanten Umgebung installiert werden sollen.  Der bereit stellungsprozess dauert bis zu 15 Minuten. Wenn die Website für den Zugriff verfügbar ist, werden Sie per e-Mail benachrichtigt (an die e-Mail-Adresse der Benachrichtigung, die Sie auf der Seite für die Einrichtung eingegeben haben). 

> [!IMPORTANT]
> Der mandantenadministrator, der die Website für Lern Pfade bereitstellt, muss zur Website wechseln und dann **CustomLearningAdmin. aspx** öffnen, um die Administrator Eigenschaften für Lern Pfade zu initialisieren. Zu diesem Zeitpunkt sollte der mandantenadministrator dem Standort auch Besitzer zuweisen. 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Überprüfen des Erfolgs der Vorstellung und Initialisieren der CustomConfig-Liste

Wenn die proprovisionierung abgeschlossen ist, erhält der mandantenadministrator, der die Website vorsieht, eine e-Mail vom PnP-Dienst für die Zustellung. Die e-Mail enthält einen Link zu der Website. An dieser Stelle sollte der mandantenadministrator die Website über den in der e-Mail angegebenen Link aufrufen und die Website für die erste Verwendung einrichten:

- Wechseln Sie zu `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`. Beim Öffnen von **CustomLearningAdmin. aspx** wird das **CustomConfig** -Listenelement initialisiert, das Lern Pfade für die erste Verwendung einrichtet. Sie sollten eine Seite sehen, die wie folgt aussieht:

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
