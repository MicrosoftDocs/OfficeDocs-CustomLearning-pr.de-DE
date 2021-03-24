---
author: pkrebs
ms.author: pkrebs
title: Bereitstellen einer neuen mehrsprachigen Lösung für Lernpfade
ms.date: 02/10/2019
description: Bereitstellen der Microsoft 365-Lernpfadwebsite über den SharePoint-Bereitstellungsdienst
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint online
ms.openlocfilehash: 19de14ba0785fa394dfe65e50ba8c4f27864cccf
ms.sourcegitcommit: 907c657e7cc5a4a44d2b9f38cc35fea9ac5c5943
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2021
ms.locfileid: "51163002"
---
# <a name="provision-a-new-learning-pathways-multilingual-solution"></a>Bereitstellen einer neuen mehrsprachigen Lösung für Lernpfade
Organisationen, die nicht über in ihrem Mandanten bereitgestellte Lernpfade verfügen, können den SharePoint-Bereitstellungsdienst verwenden, um die Lösung für mehrsprachige Lernpfade hinzuzufügen. Mit dieser Option wird die SharePoint-Vorlage für Lernpfade in neun Sprachen übersetzt und kann mit einer minimalen Änderung verwendet werden. 

> [!IMPORTANT]
> Wenn Sie bereits Lernpfade in Ihrem Mandanten bereitgestellt haben, [](custom_update_ml.md) wird empfohlen, den Aktualisierungspfad für Lernpfade zu befolgen. Wenn Sie Lernpfade über eine vorhandene Instanz in Ihrem Mandanten installieren, gehen änderungen an der Websitevorlage oder den Wiedergabelisten der Lernpfade möglicherweise verloren.

## <a name="prerequisites-for-multilingual-support"></a>Voraussetzungen für mehrsprachigen Support
 
Um Microsoft 365-Lernpfade erfolgreich mit dem Bereitstellungsdienst einrichten zu können, muss die Person, die die Bereitstellung vor sich hat, die folgenden Voraussetzungen erfüllen: 
 
- Die Person, die Lernpfade bereitstellen, muss ein Mandantenadministrator des Mandanten sein, in dem Lernpfade bereitgestellt werden.  
- Ein Mandanten-App-Katalog muss in der Option Apps des SharePoint Admin Center verfügbar sein. Wenn Ihre Organisation keinen SharePoint-Mandanten-App-Katalog hat, lesen Sie die [SharePoint](/sharepoint/use-app-catalog) Online-Dokumentation, um einen zu erstellen. Sie müssen mindestens zwei Stunden nach dem Erstellen des App-Katalogs warten, bevor Sie Lernpfade bereitstellen.  
- Die Person, die Lernpfade bereitstellen, muss ein Websitesammlungsbesitzer des Mandanten-App-Katalogs sein. Wenn die Person, die Lernpfade bereitstellen, kein Websitesammlungsbesitzer des App-Katalogs ist, führen Sie [diese](addappadmin.md) Anweisungen aus, und fahren Sie fort. 

## <a name="ensure-the-tenant-admin-account-doesnt-have-a-language-selected"></a>Sicherstellen, dass für das Mandantenadministratorkonto keine Sprache ausgewählt ist
Stellen Sie vor der Bereitstellung von Lernpfaden sicher, dass für das Administratorkonto für den Mandanten keine Sprache ausgewählt ist. Hier erfahren Sie, wie Sie überprüfen, ob für das Administratorkonto keine Sprache ausgewählt ist. 
1.  Wechseln Sie mit Ihrem Edgeadministratorprofil zu office.com.
2.  Geben Sie die Benutzeranmeldeinformationen ein (falls erforderlich).
3.  Klicken Sie in Microsoft 365 auf **Alle Apps** > Delve. 
4.  Klicken Sie **auf Me**  >  **Update Profile**.
5.  Scrollen Sie auf der Seite nach unten, und klicken **Sie auf Wie kann ich die Sprach- und Regionaleinstellungen ändern.**
6.  Klicken **Sie hier**, und klicken Sie dann auf die Ellipsen **...**.
7.  Unter **Meine Anzeigesprachen** sollte Keine **Sprachen ausgewählt angezeigt werden.** Wenn eine Sprache ausgewählt ist, deaktivieren Sie die Auswahl.

### <a name="to-provision-learning-pathways"></a>So bereitstellen Sie Lernpfade

1. Wechseln Sie zur [Lösungsseite für Microsoft 365-Lernpfade.](https://provisioning.sharepointpnp.com/details/3df8bd55-b872-4c9d-88e3-6b2f05344239)
2. Klicken **Sie auf Zu Ihrem Mandanten hinzufügen**. Wenn Sie nicht bei Ihrem Mandanten angemeldet sind, fordert der Bereitstellungsdienst Ihre Mandantenadministratoranmeldeinformationen an. 
3. Wählen Sie im Dialogfeld Angeforderte Berechtigungen die Option **Zustimmung im** Namen Ihrer Organisation aus, und wählen Sie dann **Akzeptieren aus.**

Der Bereitstellungsdienst benötigt diese Berechtigungen, um den Mandanten-App-Katalog zu erstellen, die Anwendung im Mandanten-App-Katalog zu installieren und die Websitevorlage zur Verfügung zu stellen. Es gibt keine gesamtwirtschaftlichen Auswirkungen auf Ihren Mandanten. Diese Berechtigungen werden explizit für die Lösungsinstallation verwendet. Sie müssen diese Berechtigungen akzeptieren, um mit der Installation fortfahren zu können.

4. Füllen Sie die Felder auf der Seite mit den Bereitstellungsinformationen entsprechend Ihrer Installation aus. Geben Sie mindestens die E-Mail-Adresse ein, an die Sie Benachrichtigungen über den Bereitstellungsprozess erhalten möchten, sowie die Ziel-URL der Website, an die die Bereitstellung erfolgen soll.  
> [!NOTE]
> Geben Sie der Ziel-URL Ihrer Website einen aussagekräftigen Namen wie beispielsweise „/Websites/MeinTraining“ oder „/Teams/Microsoft365Infos".

![inst_options.png](media/inst_options.png)

6. Klicken **Sie auf Bereitstellen,** wenn Sie Lernpfade in Ihrer Mandantenumgebung installieren möchten.  Der Bereitstellungsvorgang kann bis zu 15 Minuten dauern. Sie werden per E-Mail benachrichtigt, wenn die Website fertiggestellt ist. 

> [!IMPORTANT]
> Der Mandantenadministrator, der die Website für Lernpfade zur Verfügung steht, muss zur Website wechseln und **dann CustomLearningAdmin.aspx** öffnen, um Die Eigenschaften von Lernpfaden zu initialisieren. Zu diesem Zeitpunkt sollte der Mandantenadministrator der Website auch Besitzer zuweisen. 

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Überprüfen des Bereitstellungserfolgs und Initialisieren der CustomConfig-Liste

Nach Abschluss der Bereitstellung erhält der Mandantenadministrator, der die Website bereitgestellt hat, eine E-Mail vom PnP-Bereitstellungsdienst. Die E-Mail enthält einen Link zur Website. An diesem Punkt sollte der Mandantenadministrator über den in der E-Mail bereitgestellten Link zur Website wechseln und die Website für die erste Verwendung einrichten:

- Wechseln Sie zu `<YOUR-SITE-COLLECTION-URL>sites/<YOUR-SITE-NAME>/SitePages/CustomLearningAdmin.aspx`. Wenn Sie **CustomLearningAdmin. aspx** öffnen, wird das Listenelement **CustomConfig** initialisiert, das die Lernpfade für die erste Verwendung einrichtet. Es sollte eine Seite angezeigt werden, die wie dies aussieht:

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Hinzufügen von Besitzern zur Website
Als Mandantenadministrator ist es unwahrscheinlich, dass Sie die Person sein werden, die die Website anpasst, sodass Sie der Website einige Besitzer zuweisen müssen. Besitzer verfügen über Administratorrechte auf der Website, damit sie Websiteseiten ändern und die Website neubranden können. Sie haben auch die Möglichkeit, Inhalte auszublenden und anzuzeigen und benutzerdefinierte Wiedergabelisten und Unterkategorien zu erstellen.  

1. Klicken Sie im Menü **SharePoint-Einstellungen** auf **Websiteberechtigungen**.
2. Klicken Sie **auf Erweiterte Berechtigungseinstellungen**.
3. Klicken Sie auf Besitzer von **Microsoft 365-Lernpfaden.**
4. Klicken **Sie auf Neue** Benutzer zu dieser Gruppe hinzufügen, und fügen Sie dann die Personen hinzu, die Besitzer sein  >  sollen. 
5. Fügen Sie in der [Nachricht Freigeben](custom_exploresite.md) einen Link zum Durchsuchen der Website hinzu, und klicken Sie dann auf **Freigeben.**

## <a name="add-translators-to-the-site"></a>Hinzufügen von Übersetzern zur Website
Wenn Sie Übersetzer für die Website verwenden, können Sie ihnen Berechtigungen zuweisen. Übersetzer benötigen Mitgliedsberechtigungen oder höher. 

## <a name="choose-options-for-using-multiple-languages-on-the-site"></a>Auswählen von Optionen für die Verwendung mehrerer Sprachen auf der Website
Der SharePoint-Bereitstellungsdienst erstellt die Lernpfadwebsite in neun Sprachen. Es gelten die folgenden Empfehlungen:
- Deaktivieren der Sprachen, die Sie nicht unterstützen möchten
- Wenn Sie eine mehrsprachige Website nicht unterstützen, deaktivieren Sie das mehrsprachige Feature. Weitere Informationen finden Sie im Abschnitt "Deaktivieren des mehrsprachigen Support" weiter weiter in diesem Thema.

### <a name="remove-languages-you-dont-want-to-support"></a>Entfernen von Sprachen, die Sie nicht unterstützen möchten
Für Organisationen, die neben der Standardsprache Englisch nur eine Sprache unterstützen möchten, wird empfohlen, nicht unterstützte Sprachen zu entfernen. 
1. Wählen Sie auf der  Website Lernpfade oben rechts auf der Seite Einstellungen aus, und wählen Sie dann **Websiteinformationen aus.**
2. Wählen Sie unten im Bereich Websiteinformationen die Option **Alle Websiteeinstellungen anzeigen aus.**
3. Wählen **Sie unter Websiteverwaltung** die Option **Spracheinstellungen aus.**
4. Verschieben Sie unter Seiten **und Nachrichten in mehrere** Sprachen übersetzen aktivieren den Umschalter auf **Ein**. Es sollte standardmäßig Ein sein.
5. Klicken Sie unter Websitesprachen hinzufügen oder entfernen auf **Entfernen,** um die Sprachen zu entfernen, die Sie für die Website nicht benötigen. Das folgende Beispiel zeigt ein Beispiel der Seite Spracheinstellungen, auf der neben der Standardsprache Englisch italienisch angezeigt wird, das für die Website unterstützt wird.

![custom_update_ml_langsettings.png](media/custom_update_ml_langsettings.png)

> [!NOTE]
> Beim Entfernen von Sprachen können Sie die Standardsprache Englisch nicht entfernen. 

### <a name="assign-translators"></a>Zuweisen von Übersetzern
Wenn Sie Seiten übersetzen möchten, weisen Sie optional einen oder mehrere Übersetzer für jede Sprache zu (mit Ausnahme der Standardsprache der Website). 
- Geben Sie **in** der Spalte Translator den Namen einer Person ein, die Sie als Übersetzer verwenden möchten, und wählen Sie dann den Namen aus der Liste aus. 

> [!NOTE]
> Jeder im Active Directory Ihrer Organisation kann als Übersetzer zugewiesen werden. Personen, die als Übersetzer zugewiesen sind, erhalten nicht automatisch die entsprechenden Berechtigungen. Wenn jemand ohne Bearbeitungsberechtigungen für eine Website versucht, auf die Website zu zugreifen, wird er zu einer Webseite weitergeleitet, auf der er Zugriff anfordern kann.

## <a name="turn-off-multilingual-support"></a>Deaktivieren des mehrsprachigen Support
Wenn Sie z. B. keine mehrsprachige Website wünschen, sollten Sie die mehrsprachige Funktion deaktivieren. 

1. Wählen Sie auf der  Website Lernpfade oben rechts auf der Seite Einstellungen aus, und wählen Sie dann **Websiteinformationen aus.**
2. Wählen Sie unten im Bereich Websiteinformationen die Option **Alle Websiteeinstellungen anzeigen aus.**
3. Wählen **Sie unter Websiteverwaltung** die Option **Spracheinstellungen aus.**
4. Verschieben Sie unter Seiten **und Nachrichten in mehrere** Sprachen übersetzen aktivieren den Umschalter auf **Ein**. Es sollte standardmäßig Ein sein.
- Wählen **Sie unter Seiten und Zu übersetzende Nachrichten aktivieren** die Option Aus aus **aus** aus. 

### <a name="add-languages"></a>Hinzufügen von Sprachen
Lernpfade unterstützen 9 Sprachen, es wird jedoch empfohlen, dass Sie nur die Sprachen hinzufügen, die Sie für die Lernpfadwebsite unterstützen müssen. Sie können langauges jederzeit hinzufügen. 
- Geben Sie unter Hinzufügen **oder Entfernen** von Websitesprachen einen Sprachnamen in **Auswählen** oder Eingeben einer Sprache ein, oder wählen Sie eine Sprache aus dem Dropdown aus. Sie können diesen Schritt wiederholen, um mehrere Sprachen hinzuzufügen. Sie können Ihrer Website jederzeit Sprachen hinzufügen oder entfernen, indem Sie zu dieser Seite zurückwechseln.