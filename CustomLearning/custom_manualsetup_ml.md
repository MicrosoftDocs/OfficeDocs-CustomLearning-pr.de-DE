---
author: pkrebs
ms.author: pkrebs
title: Manuelle Einrichtung von Lernpfaden für ml
ms.date: 02/10/2019
description: Manuelle Einrichtung von Lernpfaden
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
ms.openlocfilehash: 386b98a49755a7dd89964446eff9d1c6cd752949
ms.sourcegitcommit: 956ab22dd8ce23ee1779f1a01d34b434243c3cb1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/11/2021
ms.locfileid: "52310379"
---
# <a name="learning-pathways-manual-setup-for-multilingual"></a>Manuelle Einrichtung von Lernpfaden für mehrsprachig

Microsoft 365 lernpfade bietet eine manuelle Einrichtung für Organisationen, die Unterstützung für eines der folgenden Szenarien benötigen:

- Ihre Organisation verfügt über eine SharePoint moderne Online-Kommunikationswebsite für Schulungen, und Sie möchten dieser Website Lernpfade hinzufügen. In diesem Szenario wurde das Web part für Lernpfade nicht auf der Website eingerichtet.

- Sie möchten Lernpfade für mehrsprachigen Support auf einer der Kommunikationswebsites SharePoint Ihrer Organisation installieren. Die Website verfügt oder hat eine Standardsprache, die nicht Englisch ist und eine der Sprachen ist, die von Lernpfaden unterstützt werden. Hier sind die Sprachen, die von Lernpfaden unterstützt werden:

- Englisch
- Chinesisch (vereinfacht)
- Französisch
- Deutsch
- Italienisch (Italien)
- Japanisch (Japan)
- Portugiesisch (Brasilien)
- Russisch (Russisch)
- Spanisch

Das manuelle Einrichten von Lernpfaden erfordert Erfahrung in Windows PowerShell und SharePoint Online Management Shell. Im Folgenden finden Sie eine Übersicht über die Schritte für die manuelle Einrichtung von Lernpfaden: 

- Überprüfen Sie, ob alle Voraussetzungen erfüllt sind.
- Überprüfen Sie die Standardspracheneinstellungen für Ihre Website. Wenn OK, fahren Sie mit der manuellen Installation fort. Wenn Sie eine andere Standardspracheneinstellung benötigen, müssen Sie eine neue Website erstellen. 
- Installieren Sie die Datei customlearning.sppkg in SharePoint Mandanten-App-Katalog.
- Bereitstellen/Identifizieren einer modernen Kommunikationswebsite, die als Microsoft 365 Lernpfade fungieren soll.
- Führen Sie ein PowerShell-Skript aus, mit dem Ihr Mandant mit den Artefakten konfiguriert wird, von den Lernpfaden abhängt.
- Navigieren Sie zur Websiteseite CustomLearningAdmin.aspx, um das Administratorwebteil zu laden, um die Konfiguration für benutzerdefinierte Inhalte zu initialisieren.

## <a name="prerequisites"></a>Voraussetzungen
Um eine erfolgreiche manuelle Einrichtung des Web teils "Lernpfade" sicherzustellen, müssen die folgenden Voraussetzungen erfüllt sein. 

- Sie müssen den mandantenweiten App-Katalog eingerichtet und konfiguriert haben. Weitere Informationen finden Sie unter Einrichten [Office 365 Mandanten,](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) und folgen Sie dem Abschnitt "App-Katalog erstellen". 
- Wenn Ihr mandantenweiter App-Katalog bereits bereitgestellt wurde, benötigen Sie Zugriff auf ein Konto, das über Rechte zum Hochladen eines Pakets verfügt. Im Allgemeinen verfügt dieses Konto SharePoint Administratorrolle. 
- Wenn ein Konto mit dieser Rolle nicht funktioniert, wechseln Sie zum SharePoint Admin Center, und suchen Sie die Websitesammlungsadministratoren für die App-Katalog-Websitesammlung, und melden Sie sich entweder als einer der Websitesammlungsadministratoren an, oder fügen Sie das SharePoint-Administratorkonto hinzu, das den Websitesammlungsadministratoren fehlgeschlagen ist. 
- Sie benötigen auch Zugriff auf ein Konto, das ein SharePoint Mandantenadministrator ist.

## <a name="step-1---check-your-language-settings"></a>Schritt 1 – Überprüfen der Spracheinstellungen
Überprüfen Sie als ersten Schritt des manuellen Installationsvorgangs die Einstellungen für die Websitesprache. Hier sind die möglichen Optionen:

### <a name="option-1---you-dont-want-multilingual-support"></a>Option 1 : Sie möchten keinen mehrsprachigen Support
Wenn Sie keinen mehrsprachigen Support für Ihre Website wünschen, stellen Sie sicher, dass sie deaktiviert ist.
1.  Wählen Sie SharePoint Kommunikationswebsite Einstellungen   >  **Websiteinformationen**  >  **Anzeigen aller Websiteeinstellungen**  >  **Spracheinstellungen aus.** 
2.  Legen Sie **die Option Seiten und Nachrichten in** mehrere Sprachen übersetzen aktivieren auf Aus **.**
3.  Klicken Sie auf **Speichern**. 
4.  Fahren Sie mit Schritt 2 fort.

## <a name="option-2---you-want-multilingual-support-and-youre-ok-with-the-default-language"></a>Option 2: Sie möchten mehrsprachigen Support und sind mit der Standardsprache in Ordnung.
Eine SharePoint kommunikationswebsite hat eine Standardsprache. Die Standardsprache bestimmt die Sprache, in der Sie Lernpfade anzeigen, einschließlich der Seite Verwaltung der Lernpfade. Die Standardspracheneinstellung wird beim ersten Erstellen der Website festgelegt und kann anschließend nicht geändert werden. Bevor Sie mit dem manuellen Setup fortfahren, stellen Sie sicher, dass Sie mit der Standardsprache der Zielwebsite in Ordnung sind.

1.  Wählen Sie SharePoint Kommunikationswebsite Einstellungen   >  **Websiteinformationen**  >  **Anzeigen aller Websiteeinstellungen**  >  **Spracheinstellungen aus.** 
2.  Legen Sie die Option Seiten **und Nachrichten in mehrere** Sprachen übersetzen aktivieren auf Ein **.**
    - Wenn Sie mit der Sprache, die oben in der Liste unter Sprache angezeigt **wird,** ok sind, können Sie weitere Sprachen hinzufügen und dann auf **Speichern klicken.** Fahren Sie mit Schritt 2 fort.
    - Wenn Sie eine andere Standardsprache als die für die Website ausgewählte Sprache wünschen, müssen Sie eine neue SharePoint-Kommunikationswebsite mit der von Ihnen benötigten Sprache erstellen. Fahren Sie mit Option 3 fort. 

## <a name="option-3---you-want-multilingual-support-but-want-a-different-default-language-for-the-site"></a>Option #3 – Sie möchten mehrsprachigen Support, aber eine andere Standardsprache für die Website
Mit dieser Option erstellen Sie eine neue SharePoint Online-Kommunikationswebsite mit der von Ihnen verwendeten Standardsprache, und legen dann die Spracheinstellungen für die Website festlegen. 
1.  Informationen zum Erstellen einer neuen SharePoint finden Sie unter [Create a communication site in SharePoint Online](https://support.microsoft.com/office/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb). Achten Sie beim Erstellen der Website darauf, die Sprache auf die Standardsprache für Lernpfade zu setzen. 
2. Wählen Sie auf der von Ihnen **erstellten Website Einstellungen**  >  **Websiteinformationen**  >  **Anzeigen aller Websiteeinstellungen**  >  **Spracheinstellungen aus.** 
2.  Legen Sie die Option Seiten **und Nachrichten in mehrere** Sprachen übersetzen aktivieren auf Ein **.**
3. Fügen Sie bei Bedarf weitere Sprachen hinzu, und klicken Sie dann auf **Speichern**. 
4. Fahren Sie mit Schritt 2 fort. 

>! [Hinweis] Wenn Sie benutzerdefinierte Inhalte von einer Website zu einer neu erstellten Website migrieren müssen, lesen Sie den Abschnitt "Benutzerdefinierte Inhalte migrieren" weiter in diesem Dokument. 

## <a name="step-2---get-the-web-part-package-and-setup-script-from-github"></a>Schritt 2 : Web part package and setup script from GitHub
Im Rahmen des Setupprozesses benötigen Sie das Microsoft 365 web part-Paket für Lernpfade und das PowerShell-Setupskript.

- Wechseln Sie [zu den Lernpfaden GitHub Repository](https://github.com/pnp/custom-learning-office-365).
- Klicken **Sie auf Herunterladen,** um das Webpartpaket und das Skript auf einem lokalen Laufwerk zu speichern. Sie verwenden das Skript und das Web part-Paket in späteren Schritten dieses Prozesses.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Schritt 2 : Hochladen des Webteils in den Mandanten-App-Katalog
Zum Einrichten Microsoft 365 Lernpfade laden Sie die Datei customlearning.sppkg in den mandantenweiten App-Katalog hoch und stellen sie zur Bereitstellung. Ausführliche Anweisungen zum Hinzufügen einer App zum App-Katalog finden Sie unter Use the App Catalog to make [custom business apps available for your SharePoint Online](/sharepoint/use-app-catalog) environment.

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>Schritt 3 – Bereitstellen/Identifizieren einer modernen Kommunikationswebsite
Identifizieren Sie entweder eine vorhandene SharePoint Oder stellen Sie eine neue in Ihrem SharePoint Online-Mandanten zur Verfügung. Weitere Informationen zum Bereitstellen einer Kommunikationswebsite finden Sie unter Erstellen einer Kommunikationswebsite [in SharePoint Online,](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) und führen Sie die Schritte zum Erstellen einer Kommunikationswebsite aus.

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>Schritt 4 : Hinzufügen der Microsoft 365 Lernpfade-App zur Website

1. Klicken Sie SharePoint auf das Menü System, und klicken Sie dann **auf App hinzufügen.** 
2. Klicken **Sie unter Ihre Apps** auf Aus Ihrer **Organisation,** und klicken Sie dann auf **Lernpfade für Office 365**. 

## <a name="step-5---set-permissions-for-the-site"></a>Schritt 5 : Festlegen von Berechtigungen für die Website
Stellen Sie sicher, dass die folgenden Berechtigungen für die Website festgelegt sind:
- **Websitesammlungsadministrator oder** Teil der Gruppe Besitzer – Erforderliche Berechtigungen zum Initialisieren des CustomConfig-Listenelements, das Lernpfade für die erste Verwendung eingerichtet. 
- **Mitgliedergruppe** – Erforderliche Berechtigungen zum Verwalten von Lernpfaden, einschließlich Ausblenden und Anzeigen von Inhalten und Verwalten benutzerdefinierter Wiedergabelisten
- **Gruppe "Besucher"** – Erforderliche Berechtigungen zum Anzeigen von Websiteinhalten. 

## <a name="step-6--execute-powershell-configuration-script"></a>Schritt 6: Ausführen des PowerShell-Konfigurationsskripts
Ein PowerShell-Skript ist enthalten, das Sie ausführen müssen, um drei Mandanteneigenschaften zu erstellen, die `CustomLearningConfiguration.ps1` von der Lösung verwendet werden. [](/sharepoint/dev/spfx/tenant-properties) Darüber hinaus erstellt das Skript zwei [einzelne Teil-App-Seiten](/sharepoint/dev/spfx/web-parts/single-part-app-pages) in der Websiteseitenbibliothek, um die Administrator- und Benutzerwebparts an einem bekannten Speicherort zu hosten.

1. Wenn Sie die SharePoint Online Management Shell noch nicht heruntergeladen haben, laden Sie sie jetzt herunter. Weitere [SharePoint finden Sie unter Download der Onlineverwaltungsshell](https://go.microsoft.com/fwlink/p/).
2. Möglicherweise müssen Sie eine PowerShell-Ausführungsrichtlinie festlegen, um das Skript auszuführen. Weitere Informationen finden Sie unter [About Execution Policies](/powershell/module/microsoft.powershell.core/about/about_execution_policies).
3. Führen Sie das `CustomLearningConfiguration.ps1` Skript aus. Zusätzlich zu Ihren Mandantenadministratoranmeldeinformationen fordert das Skript Sie auf, Ihren Mandantennamen und Websitenamen ein. Unter Berücksichtigung des folgenden Beispiels für Ihre Website-URL ist `https://contoso.sharepoint.com/sites/O365CL` , `contoso` der Mandantenname und der `O365CL` Websitename. 

### <a name="disabling-telemetry-collection"></a>Deaktivieren der Telemetriesammlung
Teil dieser Lösung ist die anonymisierte Telemetrieverfolgung, die standardmäßig auf ein festgelegt ist. Wenn Sie eine manuelle Installation ausführen und die Telemetrieverfolgung deaktivieren möchten, ändern Sie das Skript so, dass die variable $optInTelemetry auf $false festgelegt wird, und führen Sie `CustomlearningConfiguration.ps1` das Skript aus.

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Überprüfen des Bereitstellungserfolgs und Initialisieren der CustomConfig-Liste

Nachdem das PowerShell-Skript erfolgreich ausgeführt wurde, navigieren Sie  zur Website, initialisieren das CustomConfig-Listenelement, das Lernpfade für die erste Verwendung eingerichtet hat, und überprüfen, ob die Website funktioniert.

- Wechseln Sie zu `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`. Wenn Sie **CustomLearningAdmin. aspx** öffnen, wird das Listenelement **CustomConfig** initialisiert, das die Lernpfade für die erste Verwendung einrichtet. Es sollte eine Seite angezeigt werden, die wie dies aussieht:

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Hinzufügen von Besitzern zur Website
Als Mandantenadministrator ist es unwahrscheinlich, dass Sie die Person sein werden, die die Website anpasst, sodass Sie der Website einige Besitzer zuweisen müssen. Besitzer verfügen über Administratorrechte auf der Website, damit sie Websiteseiten ändern und die Website neubranden können. Sie haben auch die Möglichkeit, Inhalte auszublenden und anzuzeigen, die über das Web part für Lernpfade übermittelt werden. Darüber hinaus können sie benutzerdefinierte Wiedergabelisten erstellen und benutzerdefinierten Unterkategorien zuweisen.  

1. Klicken Sie im SharePoint **Einstellungen** auf **Websiteberechtigungen**.
2. Klicken **Sie auf Erweiterte Berechtigung Einstellungen**.
3. Klicken **Sie auf Lernpfade für Office 365 Besitzer**.
4. Klicken **Sie auf Neue** Benutzer zu dieser Gruppe hinzufügen, und fügen Sie dann die Personen hinzu, die Besitzer sein  >  sollen. 
5. Fügen Sie in der [Nachricht Freigeben](custom_exploresite.md) einen Link zum Durchsuchen der Website hinzu, und klicken Sie dann auf **Freigeben.**

## <a name="migrate-custom-content"></a>Migrieren benutzerdefinierter Inhalte
Nachdem Sie Ihre Lernpfade-Website anhand der oben beschriebenen Schritte wieder eingerichtet haben, müssen Sie den Inhalt Ihrer Listen **CustomPlaylists** und **CustomAssets** verschieben. Sie können optional auch die tatsächlichen benutzerdefinierten Seiten, aus denen sich Ihre benutzerdefinierten Objekte zusammensetzen, verschieben, wenn sie in der bestehenden Lernpfade-Website vorhanden sind und Sie beabsichtigen, sie zu löschen. Die Aufgabe kann schwierig sein, da für alle Elemente in der Liste **CustomPlaylists** die ID des Listenelements in der Liste **CustomAssets** im Feld "JSONData" des jeweiligen Wiedergabelistenelements verborgen ist. Das einfache Verschieben des Inhalts der **Liste "CustomPlaylists"** von einer Website zur anderen reicht also nicht aus. Außerdem enthält die Liste **CustomAssets** die absolute URL für die Seite des benutzerdefinierten Objekts im Feld "JSONData" des Listenelements. Wenn die Objekte nicht verschoben werden und die Website nicht umbenannt (also die absolute URL der Seite des Objekts geändert) wird, kann **CustomAssets** beibehalten werden. Sie müssen die Einträge aber manuell korrigieren. Angesichts der Komplexität dieser Art von Migration sollten Sie erwägen, einen unserer Lernpfade-Partner in Anspruch zu nehmen, um Ihnen bei der Durchführung dieses Übergangs zu helfen. 

### <a name="next-steps"></a>Nächste Schritte
- Weitere [Informationen finden Sie unter Customize learning pathways](custom_overview.md). 
- Weitere [Informationen finden Sie unter Übersetzen von Websiteseiten](custom_translate_page_ml.md).