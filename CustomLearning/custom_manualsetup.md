---
author: pkrebs
ms.author: pkrebs
title: Eigenständiges Webpart-Setup
ms.date: 02/10/2019
description: Microsoft 365 Lern Pfade Manuelles Webpart-Setup
ms.openlocfilehash: f3271dbd75ee18db7f89fdd15ebb35c1b2bf7d97
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/21/2019
ms.locfileid: "34247870"
---
# <a name="stand-alone-web-part-setup"></a>Eigenständiges Webpart-Setup

Microsoft 365 Learning-Pfade bietet eine manuelle, eigenständige WebPart-Einrichtung für Organisationen, die bereits über eine etablierte SharePoint Online moderne Kommunikationswebsite verfügen, die für die Schulung vorgesehen ist, oder die einfach das Webpart "Lernpfade" in einrichten möchten. eigene Kommunikationswebsite. Beachten Sie, dass das manuelle Setup eine Erfahrung in der Arbeit mit Windows PowerShell und der SharePoint Online Management-Shell erfordert. Die Schritte für eine manuelle Einrichtung des Webparts Lernpfade folgendermaßen:

- Überprüfen Sie, ob Sie alle Voraussetzungen erfüllt haben.
- Installieren Sie die Datei customlearning. sppkg in Ihrem SharePoint-Mandanten-App-Katalog.
- Stellen Sie eine moderne Kommunikationswebsite zur Verfügung, die Sie als Microsoft 365-Lern Pfade als Startseite fungieren möchten.
- Führen Sie ein PowerShell-Skript aus, mit dem Ihr Mandant mit den entsprechenden Artefakten konfiguriert wird, von denen Lern Pfade abhängen.
- Navigieren Sie zur Seite CustomLearningAdmin. aspx, um das Admin-Webpart zu laden, um die benutzerdefinierte Inhalts Konfiguration zu initialisieren.

> [!NOTE]
> Wenn Sie eine schnelle und einfache Möglichkeit zum Einrichten von Lernpfaden benötigen, finden Sie weitere Informationen unter [Microsoft 365-Lern Pfade](custom_provision.md).

## <a name="prerequisites"></a>Voraussetzungen
Um eine erfolgreiche manuelle Einrichtung des Webparts für Lern Pfade sicherzustellen, müssen die folgenden Voraussetzungen erfüllt sein. 

- Sie müssen den Mandanten weiten App-Katalog eingerichtet und konfiguriert haben. Weitere Informationen finden Sie unter [Einrichten des Office 365 Mandanten](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) und dem Abschnitt Erstellen der APP-katalogwebsite. 
- Wenn Ihr Mandanten weiter App-Katalog bereits bereitgestellt wurde, benötigen Sie Zugriff auf ein Konto, das über Rechte zum Hochladen eines Pakets verfügt, damit dieser Setupvorgang abgeschlossen wird. Im Allgemeinen handelt es sich hierbei um ein Konto mit der SharePoint-Administratorrolle. 
- Wenn ein Konto mit dieser Rolle nicht funktioniert, wechseln Sie zum SharePoint Admin Center, suchen Sie die Websitesammlungsadministratoren für die APP-Katalog-Websitesammlung, und melden Sie sich entweder als einer der Websitesammlungsadministratoren an, oder fügen Sie das SharePoint-Administratorkonto hinzu. Fehler bei den Websitesammlungsadministratoren. 
- Sie benötigen auch Zugriff auf ein Konto, bei dem es sich um einen SharePoint-mandantenadministrator handelt.

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>Schritt 1: Abrufen des Webpart-Pakets und des Setupskripts von GitHub
Im Rahmen des Setupprozesses benötigen Sie das Microsoft 365 Learning-Pfad-Webpart-Paket und das PowerShell-Setupskript.

- Wechseln Sie zum [Repository für Lern Pfade GitHub](https://github.com/pnp/custom-learning-office-365).
- Klicken Sie auf **herunterladen** , um das Webparts-Paket und das Skript auf einem lokalen Laufwerk zu speichern. Sie verwenden das Skript und das Webpart-Paket in späteren Schritten dieses Prozesses.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Schritt 2: Hochladen des Webparts in den Mandanten-App-Katalog
Um Microsoft 365-Lern Pfade einzurichten, laden Sie die Datei customlearning. sppkg in den Mandanten weiten App-Katalog hoch und stellen Sie bereit. Ausführliche Anweisungen zum Hinzufügen einer App zum App-Katalog finden Sie unter [Verwenden des App-Katalogs, um benutzerdefinierte Business-Apps für Ihre SharePoint Online Umgebung zur Verfügung zu stellen](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) .

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>Schritt 3 – Bereitstellung/Identifizierung einer modernen Kommunikationswebsite
Identifizieren Sie entweder eine vorhandene SharePoint-Kommunikationswebsite, oder stellen Sie eine neue in Ihrem SharePoint Online Mandanten zur Verfügung. Weitere Informationen zum Einrichten einer Kommunikationswebsite finden Sie unter [Create a Communication Site in SharePoint Online](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) und folgen den Schritten zum Erstellen einer Kommunikationswebsite.

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>Schritt 4 – Hinzufügen der App "Microsoft 365 Learning Pfads" zur Website

1. Klicken Sie auf der SharePoint-Website auf das Menü System, und klicken Sie dann auf **app hinzufügen**. 
2. Klicken Sie unter **Ihre apps**auf **aus Ihrer Organisation**, und klicken Sie dann auf **Lern Pfade für Office 365**. 

## <a name="step-5---set-permissions-for-the-site"></a>Schritt 5 – Festlegen von Berechtigungen für die Website
Stellen Sie sicher, dass die folgenden Berechtigungen für die Website festgelegt sind:
- **Website Sammlungs Administrator oder Teil der Gruppe Besitzer** – erforderliche Berechtigungen zum Initialisieren des CustomConfig-Listenelements, das Lern Pfade für die erste Verwendung einrichtet. 
- **Mitgliedergruppe** – PERMISSONS, die zum Verwalten von Lernpfaden erforderlich sind, einschließlich ausblenden und Anzeigen von Inhalten und Verwalten benutzerdefinierter Wiedergabelisten
- **Besuchergruppe** – für die Anzeige von Websiteinhalten sind Berechtigungen erforderlich. 

## <a name="step-6--execute-powershell-configuration-script"></a>Schritt 6-Ausführen des PowerShell-Konfigurationsskripts
Ein PowerShell- `CustomLearningConfiguration.ps1` Skript ist enthalten, das Sie ausführen müssen, um drei [Mandanten Eigenschaften](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) zu erstellen, die von der Lösung verwendet werden. Darüber hinaus erstellt das Skript zwei [einzelne Teile-App-Seiten](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) in der Bibliothek Website Seiten, um die Administrator-und Benutzer Webparts an einem bekannten Speicherort zu hosten.

1. Wenn Sie die SharePoint Online Management-Shell noch nicht heruntergeladen haben, laden Sie Sie jetzt herunter. Weitere Informationen finden Sie unter [SharePoint Online Management Shell Download](https://go.microsoft.com/fwlink/p/?LinkId=255251).
2. Möglicherweise müssen Sie eine PowerShell-Ausführungsrichtlinie festlegen, um das Skript auszuführen. Weitere Informationen finden Sie unter [Informationen zu Ausführungsrichtlinien](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).
3. Führen Sie `CustomLearningConfiguration.ps1` das Skript aus. Zusätzlich zu den Anmeldeinformationen für den mandantenadministrator werden Sie vom Skript aufgefordert, ihren Mandantennamen und den Websitenamen einzugeben. In Anbetracht des folgenden Beispiels für Ihre Website `https://contoso.sharepoint.com/sites/O365CL`- `contoso` URL ist der Name des `O365CL` Mandanten und der Name der Website. 

### <a name="disabling-telemetry-collection"></a>Deaktivieren der Telemetrie-Sammlung
Ein Teil dieser Lösung umfasst die anonymisierte Telemetrie-Überwachung Opt in, die standardmäßig auf ein festgelegt ist. Wenn Sie eine manuelle Installation durchführen und die Telemetrie-Verfolgung deaktivieren möchten, ändern Sie das `CustomlearningConfiguration.ps1` Skript, um die $optInTelemetry Variable auf $false und das Skript auszuführen.

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Überprüfen des Erfolgs der Vorstellung und Initialisieren der CustomConfig-Liste

Nachdem das PowerShell-Skript erfolgreich ausgeführt wurde, navigieren Sie zur Website, initialisieren das **CustomConfig** -Listenelement, das Lern Pfade für die erste Verwendung einrichtet, und überprüfen, ob die Website funktioniert.

- Navigieren Sie in das Verzeichnis `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`. Beim Öffnen von **CustomLearningAdmin. aspx** wird das **CustomConfig** -Listenelement initialisiert, das Lern Pfade für die erste Verwendung einrichtet. Sie sollten eine Seite sehen, die wie folgt aussieht:

![CG-adminapppage. png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Hinzufügen von Besitzern zur Website
Als mandantenadministrator ist es unwahrscheinlich, dass Sie die Person anpassen, die die Website anpasst, sodass Sie der Website einige Besitzer zuweisen müssen. Besitzer verfügen über Administratorrechte für die Website, damit Sie Website Seiten ändern und die Website neu Branding können. Außerdem können Sie Inhalte, die über das Lern Pfade-Webpart übermittelt werden, ausblenden und anzeigen. Darüber hinaus haben Sie die Möglichkeit, benutzerdefinierte Wiedergabelisten zu erstellen und Sie benutzerdefinierten Unterkategorien zuzuweisen.  

1. Klicken Sie im Menü SharePoint- **Einstellungen** auf **Websiteberechtigungen**.
2. Klicken Sie auf **Erweiterte Berechtigungseinstellungen**.
3. Klicken Sie auf **Lern Pfade für Office 365 Besitzer**.
4. Klicken Sie auf **neu** > **Hinzufügen von Benutzern zu dieser Gruppe**, und fügen Sie dann die Personen hinzu, die Besitzer sein sollen. 
5. Fügen Sie einen Link zum [Durchsuchen der Website](https://docs.microsoft.com/en-us/Office365/CustomLearning/custom_explore) in der Freigabenachricht hinzu, und klicken Sie dann auf **Freigeben**.

### <a name="next-steps"></a>Nächste Schritte
- [Passen](custom_overview.md) Sie die Schulungserfahrung für Ihre Organisation an.

