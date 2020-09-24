---
author: pkrebs
ms.author: pkrebs
title: Stellen Sie die benutzerdefinierte Lernwebsite zur Verfügung
ms.date: 02/10/2019
description: Stellen Sie das benutzerdefinierte Lernprogramm für Office 365 Website über das SharePoint-Bereitstellungsmodul zur Verfügung.
ms.service: sharepoint online
ms.openlocfilehash: feebef7f351aab4cd1efe7f87596dad98dba7536
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/23/2020
ms.locfileid: "48233757"
---
# <a name="provision-custom-learning"></a>Benutzerdefiniertes Lernen anbieten

Mit dem SharePoint Online-Bereitstellung-Dienst kann ein Office 365-Mandanten Administrator den Bereitstellung-Prozess mit wenigen einfachen Klicks starten. Der Bereitstellungsdienst ist die empfohlene Vorgehensweise zur Erstellung benutzerdefinierter Lernmethoden. Es ist schnell, einfach und dauert nur ein paar Minuten, um den Prozess zu starten. Stellen Sie jedoch sicher, dass Sie die Voraussetzungen für die Bereitstellung erfüllt haben, bevor Sie mit dem Bereitstellung-Dienst beginnen.

## <a name="prerequisites"></a>Voraussetzungen
 
Für eine erfolgreiche Einrichtung des benutzerdefinierten Lernens mit dem [SharePoint Online-Dienst](https://provisioning.sharepointpnp.com)für die Dienstleistung "Provision" muss die Person, die die proprovisionierung ausführt, die folgenden Voraussetzungen erfüllen: 
 
- Die Person, die benutzerdefiniertes lernen vorsieht, muss ein Mandant Administratorof dem Mandanten sein, in dem benutzerdefinierte Lernprozesse vorgesehen werden.  
- Ein Mandanten-App-Katalog muss in der apps-Option des SharePoint Admin Center verfügbar sein. Wenn Ihre Organisation nicht über einen SharePoint-Mandanten-App-Katalog verfügt, lesen Sie in der [SharePoint Online Dokumentation](https://docs.microsoft.com/sharepoint/use-app-catalog) nach, um eine zu erstellen.  
- Die Person, die benutzerdefiniertes lernen vorsieht, muss ein Websitesammlungsbesitzer des Mandanten-App-Katalogs sein. Wenn die Person, die benutzerdefiniertes lernen anbietet, kein Websitesammlungsbesitzer des App-Katalogs ist, [führen Sie diese Anweisungen](addappadmin.md) aus, und fahren Sie fort. 

### <a name="to-provision-custom-learning"></a>So stellen Sie benutzerdefiniertes Lernen zur Verfügung

1. Wechseln Sie zu, http://provisioning.sharepointpnp.com und **melden** Sie sich von der oberen rechten Ecke der Startseite aus an.  Melden Sie sich mit den Anmeldeinformationen für den Zielmandanten an, in dem Sie die Websitevorlage installieren möchten.

![pnphome.png](media/inst_signin.png)

2. Löschen Sie die **Zustimmung im Namen Ihrer Organisation** , und wählen Sie **annehmen**aus.

![in](media/inst_perms.png)

3. Wählen Sie **benutzerdefiniertes lernen für Office 365** aus dem Lösungskatalog aus.

![in](media/inst_select.png)

4. Wählen Sie auf der Startseite der Lösung die Option **zu Ihrem Mandanten hinzufügen** aus.

![inst_select.png](media/inst_add.png)

5. Füllen Sie die Felder auf der Seite mit den Bereitstellungsinformationen entsprechend Ihrer Installation aus. Geben Sie mindestens die e-Mail-Adresse ein, unter der Sie Benachrichtigungen über den Bereitstellung-Prozess und die Ziel-URL für die Bereitstellung Ihrer Website erhalten möchten.  
> [!NOTE]
> Stellen Sie die Ziel-URL für Ihre Website so freundlich wie "/Sites/MyTraining" oder "/Teams/LearnOffice365" für Ihre Mitarbeiter dar.

![inst_options.png](media/inst_options.png)

6. Wählen Sie **bereit** stellen aus, wenn Sie benutzerdefiniertes lernen in Ihrer Mandanten Umgebung installieren möchten.  Der Bereitstellungsvorgang kann bis zu 15 Minuten dauern. Sie werden per E-Mail (an die Benachrichtigungs-E-Mail-Adresse, die Sie auf der Seite "Bereitstellung" eingegeben haben) benachrichtigt, wenn die Website für den Zugriff bereit ist.

> [!IMPORTANT]
> Der mandantenadministrator, der die benutzerdefinierte Lernwebsite bereitstellt, muss zur Website wechseln und dann CustomLearningAdmin. aspx öffnen, um benutzerdefinierte Lern Administrator Eigenschaften zu initialisieren. Zu diesem Zeitpunkt sollte der mandantenadministrator dem Standort auch Besitzer zuweisen. 

## <a name="validate-provisioning-success"></a>Überprüfen des Erfolgs der Vorstellung

Wenn die Einrichtung abgeschlossen ist, erhält der mandantenadministrator vom PnP-Dienst eine e-Mail. Der Administrator kann den Link zu der in der e-Mail angegebenen Website kopieren und dann den Anweisungen folgen, um zur Website zu wechseln. Alternativ kann der mandantenadministrator zu <Your-Site-Collection-URL>/SitePages/customlearningadmin.aspx. navigieren. Dadurch wird das CustomConfig-Listenelement initialisiert, mit dem benutzerdefiniertes lernen für die erste Verwendung eingerichtet wird. Die Person, die diese Seite zuerst öffnet, muss ein mandantenadministrator, Websitesammlungsadministrator oder Besitzer der Website sein. Sie sollten eine Seite sehen, die wie folgt aussieht: 

## <a name="add-owners-to-site"></a>Hinzufügen von Besitzern zur Website
Als mandantenadministrator ist es unwahrscheinlich, dass Sie die Person anpassen, die die Website anpasst, sodass Sie der Websitebesitzer zuweisen müssen. Besitzer verfügen über Administratorrechte für die Website, damit Sie Website Seiten ändern und die Website neu Branding können. Sie haben auch die Möglichkeit, Inhalte, die über das benutzerdefinierte Lern Webpart übermittelt werden, auszublenden und anzuzeigen. Sie haben außerdem die Möglichkeit, benutzerdefinierte Wiedergabelisten zu erstellen und Sie benutzerdefinierten Unterkategorien zuzuweisen.  

1. Klicken Sie im Menü SharePoint- **Einstellungen** auf **Websiteberechtigungen**.
2. Klicken Sie auf **Erweiterte Berechtigungseinstellungen**.
3. Klicken Sie auf **benutzerdefiniertes lernen für Office 365 Besitzer**.
4. Klicken Sie auf **neue**  >  **Benutzer zu dieser Gruppe hinzufügen**, fügen Sie die Personen hinzu, die Besitzer sein sollen, und klicken Sie dann auf **Freigeben**.

8. Klicken Sie auf die **folgende** Option in der oberen rechten Ecke der Seite, um der Website zu folgen.  

### <a name="next-steps"></a>Nächste Schritte
- Untersuchen Sie den im Webpart enthaltenen [Standardinhalt](sitecontent.md) .
