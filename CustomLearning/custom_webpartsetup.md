---
author: pkrebs
ms.author: pkrebs
title: Einrichten der benutzerdefinierten Lernsite
ms.date: 02/10/2019
description: Stellen Sie die benutzerdefinierte Learning for Office 365-Website über das SharePoint-bereitstellungsModul zur Verfügung.
ms.openlocfilehash: 83d76d2d12e9dfc0f39ef55c58443cb3fda2a2d9
ms.sourcegitcommit: e0adc8963419a4dd5c4d9bcc9f4f2cc1fbe291d4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2019
ms.locfileid: "30523594"
---
# <a name="provision-custom-learning"></a>Benutzerdefiniertes lernen einrichten

Mit dem SharePoint Online-proplanungs Dienst kann ein Office 365-Mandanten Administrator den proplanungs Prozess mit ein paar einfachen Klicks starten. Der bereitstellungsDienst ist die empfohlene Methode zum Einrichten von benutzerdefiniertem lernen. Es ist schnell, einfach und dauert nur ein paar Minuten, um den Prozess zu starten. Bevor Sie mit dem proSupporting-Dienst beginnen, sollten Sie sich jedoch vergewissern, dass Sie die Voraussetzungen für die bereit legung erfüllt haben.

## <a name="prerequisites"></a>Voraussetzungen
 
Um benutzerdefiniertes lernen erfolgreich mit dem [SharePoint Online-](https://provisioning.sharepointpnp.com)proArbeits Dienst für die Einrichtung einrichten zu können, muss die Person, die die proversionierung durchführen soll, die folgenden Voraussetzungen erfüllen: 
 
- Die benutzerdefinierte Lernumgebung muss ein Mandant Administratorof dem Mandanten sein, in dem benutzerdefiniertes lernen eingerichtet wird.  
- Ein Mandanten-App-Katalog muss in der apps-Option im SharePoint Admin Center verfügbar sein. Wenn Ihre Organisation keinen SharePoint-Mandanten-App-Katalog hat, lesen Sie die [SharePoint Online-Dokumentation](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) , um eine zu erstellen.  
- Die benutzerdefinierte Schulung für Personen muss ein WebsitesammlungsBesitzer des Mandanten-App-Katalogs sein. Wenn die Person, die benutzerdefiniertes lernen anbietet, kein WebsitesammlungsBesitzer des App-Katalogs ist, führen Sie die [folgenden Anweisungen](addappadmin.md) aus, und fahren Sie fort. 

### <a name="to-provision-custom-learning"></a>So können Sie benutzerdefiniertes lernen einrichten

1. Wechseln Sie http://provisioning.sharepointpnp.com zu und melden Sie sich **in** der oberen rechten Ecke der Startseite an.  Melden Sie sich mit den Anmeldeinformationen für den Zielmandanten an, in dem Sie die Websitevorlage installieren möchten.

![pnphome. png](media/inst_signin.png)

2. Löschen Sie die **Einwilligung im Namen Ihrer Organisation** , und wählen Sie **akzeptieren**aus.

![in](media/inst_perms.png)

3. Wählen Sie **BenutzerdefiniertEs lernen für Office 365** aus dem Lösungskatalog aus.

![in](media/inst_select.png)

4. Wählen Sie auf der Startseite der Lösung **Ihrem mandantEn hinzufügen** aus.

![inst_select. png](media/inst_add.png)

5. Füllen Sie die Felder auf der Seite proinformations Informationen entsprechend Ihrer Installation aus. Geben Sie mindestens die e-Mail-Adresse ein, unter der Sie Benachrichtigungen über den proplanungs Prozess und die Ziel-URL für Ihre Website erhalten möchten.  
> [!NOTE]
> Stellen Sie die Ziel-URL Ihrer Website für Ihre Mitarbeiter wie "/sites/MyTraining" oder "/teams/LearnOffice365" bereit.

![inst_options. png](media/inst_options.png)

6. Wählen Sie **bereit** stellen, wenn Sie bereit sind, benutzerdefiniertes lernen in Ihre Mandanten Umgebung zu installieren.  Das Bereitstellen dauert bis zu 15 Minuten. Sie werden per e-Mail (an die Benachrichtigungs-e-Mail-Adresse, die Sie auf der Seite Bereitstellung eingegeben haben) benachrichtigt, wenn die Website auf den Zugriff zugreifen kann.

> [!IMPORTANT]
> Der MandantenAdministrator, der die benutzerdefinierte Lernsite bereitstellt, muss zur Website wechseln und dann CustomLearningAdmin. aspx öffnen, um benutzerdefinierte Learning admin-Eigenschaften zu initialisieren. Zu diesem Zeitpunkt sollte der MandantenAdministrator auch Besitzer der Website zuweisen. 

## <a name="validate-provisioning-success"></a>ÜberPrüfen des Erfolgs der überPrüfung

Wenn die Einrichtung abgeschlossen ist, erhält der MandantenAdministrator eine e-Mail vom PnP-proarbeits Dienst. Der Administrator kann den Link zu der in der e-Mail bereitgestellten Website kopieren und dann den Anweisungen folgen, um zur Website zu wechseln. Alternativ kann der mandantenadministrator zu <YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin. aspx navigieren. Dadurch wird das CustomConfig-Listenelement initialisiert, das benutzerdefiniertes lernen für die erste Verwendung festlegt. Die Person, die diese Seite zum ersten Mal öffnet, muss ein MandantenAdministrator, ein WebsitesammlungsAdministrator oder ein Besitzer der Website sein. Es sollte eine Seite angezeigt werden, die wie folgt aussieht: 

## <a name="add-owners-to-site"></a>Hinzufügen von Besitzern zur Website
Als MandantenAdministrator ist es unwahrscheinlich, dass Sie die Website anpassen, daher müssen Sie der Websitebesitzer zuweisen. Besitzer verfügen über Administratorrechte für die Website, damit Sie Website Seiten ändern und die Website neu bebranden können. Außerdem können Sie Inhalte, die über das benutzerdefinierte Lern Webpart übermittelt werden, ausblenden und anzeigen. Sie haben auch die Möglichkeit, benutzerdefinierte Wiedergabelisten zu erstellen und Sie benutzerdefinierten Unterkategorien zuzuweisen.  

1. Klicken Sie im Menü SharePoint- **Einstellungen** auf **Websiteberechtigungen**.
2. Klicken Sie auf **Erweiterte Berechtigungseinstellungen**.
3. Klicken Sie auf **benutzerdefiniertes lernen für Office 365-Besitzer**.
4. Klicken Sie auf **neue** > **Benutzer zu dieser Gruppe hinzufügen**, fügen Sie die Personen hinzu, die Besitzer sein sollen, und klicken Sie dann auf **Freigeben**.

8. Klicken Sie in der oberen rechten Ecke der Seite auf die **folgende** Option, um der Website zu folgen.  

### <a name="next-steps"></a>Weitere Schritte
- Erkunden Sie die im Webpart enthaltenen [Standardinhalte](sitecontent.md) .
