---
author: pkrebs
ms.author: pkrebs
title: Eigenständiges Webpart-Setup
ms.date: 02/10/2019
description: Benutzerdefiniertes Learning for Office 365 Manual-Webpart-Setup
ms.openlocfilehash: f5d94d673f491d5b5778ef73d518914dbd4cdbb9
ms.sourcegitcommit: e0adc8963419a4dd5c4d9bcc9f4f2cc1fbe291d4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2019
ms.locfileid: "30523059"
---
# <a name="stand-alone-web-part-setup"></a>Eigenständiges Webpart-Setup

Custom Learning bietet ein manuelles, eigenständiges Webpart-Setup für Organisationen, die bereits über eine etablierte SharePoint Online-Website für moderne Kommunikation verfügen, die für Schulungen vorgesehen ist oder die nur das benutzerdefinierte Lern Webpart in ihren eigenen einrichten möchten. Kommunikationswebsite. Beachten Sie, dass die manuelle Einrichtung Erfahrung mit Windows PowerShell und der SharePoint Online-Verwaltungsshell erfordert. Die Schritte für eine manuelle Einrichtung des benutzerdefinierten Lern Webparts wie folgt:

- Überprüfen Sie, ob alle Voraussetzungen erfüllt sind.
- Installieren Sie die Datei customlearning. sppkg im Office 365-Mandanten-App-Katalog.
- Stellen Sie eine moderne Kommunikationswebsite zur Verfügung, die als benutzerdefiniertes Learning für Office 365-Homepage dient.
- Führen Sie ein PowerShell-Skript aus, das den Mandanten mit den entsprechenden Artefakten konfiguriert, von denen die benutzerdefinierte Schulung abhängig ist.
- Navigieren Sie zur Seite CustomLearningAdmin. aspx, um das Admin-Webpart zu laden, um die benutzerdefinierte Inhalts Konfiguration zu initialisieren.

> [!NOTE]
> Wenn Sie nach einer schnellen, einfachen Methode zum Einrichten von benutzerdefiniertem lernen suchen, finden Sie weitere Informationen unter " [BenutzerdefiniertEs lernen](installsitepackage.md)".

## <a name="prerequisites"></a>Voraussetzungen
Um eine erfolgreiche manuelle Einrichtung des benutzerdefinierten Lern Webparts sicherzustellen, müssen die folgenden Voraussetzungen erfüllt sein. 

- Sie müssen den Mandanten weiten App-Katalog eingerichtet und konfiguriert haben. Weitere Informationen finden Sie unter [Einrichten Ihres Office 365](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) -Mandanten und folgen Sie dem Abschnitt Erstellen einer APP-katalogwebsite. 
- Wenn Ihr Mandanten weiter App-Katalog bereits bereitgestellt wurde, benötigen Sie Zugriff auf ein Konto, das über die Berechtigung zum Hochladen eines Pakets zum Ausführen dieses Setupvorgangs verfügt. Im Allgemeinen handelt es sich um ein Konto mit der SharePoint-Administratorrolle. 
- Wenn ein Konto mit dieser Rolle nicht funktioniert, wechseln Sie zum SharePoint Admin Center, suchen Sie die WebsitesammlungsAdministratoren für die Websitesammlung des App-Katalogs, und melden Sie sich als einer der WebsitesammlungsAdministratoren an, oder fügen Sie das SharePoint-Administratorkonto hinzu. , die den WebsitesammlungsAdministratoren nicht gelungen sind. 
- Sie benötigen außerdem Zugriff auf ein Konto, das ein SharePoint-MandantenAdministrator ist.

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>Schritt 1: Abrufen des Webpart-Pakets und des Setupskripts von GitHub
Im Rahmen des Setupvorgangs benötigen Sie das benutzerdefinierte Lern Webpart-Paket und das PowerShell-Setupskript.

- Gehen Sie zum [benutzerdefinierten Lern-GitHub-Repository](https://github.com/pnp/custom-learning-office-365).
- Klicken Sie auf **herunterladen** , um das Webpart-Paket und das Skript auf einem lokalen Laufwerk zu speichern. Sie verwenden das Skript und das Webpart-Paket in späteren Schritten dieses Prozesses.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Schritt 2: Hochladen des Webparts in den Mandanten-App-Katalog
Zum Einrichten von benutzerdefiniertem lernen für Office 365 laden Sie die Datei customlearning. sppkg in den Mandanten weiten App-Katalog hoch und stellen Sie bereit. Weitere Informationen zum Hinzufügen einer App zum App-Katalog finden Sie unter [Verwenden des App-Katalogs, um benutzerdefinierte Geschäfts-Apps für Ihre SharePoint Online-Umgebung](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) zur Verfügung zu stellen.

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>Schritt 3-Bestimmung/Identifizierung einer modernen Kommunikationswebsite
Identifizieren Sie eine vorhandene SharePoint-Kommunikationswebsite, oder stellen Sie eine neue in Ihrem SharePoint Online-Mandanten ein. Weitere Informationen zum Einrichten einer Kommunikationswebsite finden Sie unter [Erstellen einer Kommunikationswebsite in SharePoint Online](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) und führen Sie die Schritte zum Erstellen einer Kommunikationswebsite aus.

## <a name="step-4---set-permissions-for-the-site"></a>Schritt 4-Festlegen von Berechtigungen für die Website
Stellen Sie sicher, dass die folgenden Berechtigungen für die Website festgelegt sind:
- **Website Sammlungs Administrator oder Teil der Gruppe der Besitzer** – Berechtigungen, die zum Initialisieren des CustomConfig-Listenelements erforderlich sind, das benutzerdefiniertes lernen für die erste Verwendung festlegt. 
- **Mitgliedergruppe** – PERMISSONS erforderlich, um benutzerdefiniertes lernen zu verwalten, einschließlich des Ausblendens und Anzeigens von Inhalten und Verwalten von benutzerdefinierten Wiedergabelisten
- **Besuchergruppe** – Berechtigungen, die zum Anzeigen von Websiteinhalten erforderlich sind. 

## <a name="step-5--execute-powershell-configuration-script"></a>Schritt 5 – Ausführen des PowerShell-Konfigurationsskripts
Ein PowerShell- `CustomLearningConfiguration.ps1` Skript ist enthalten, das Sie ausführen müssen, um drei [Mandanten Eigenschaften](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) zu erstellen, die die Lösung verwendet. Darüber hinaus erstellt das Skript zwei [einzelne Teile-App-Seiten](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) in der Bibliothek für Website Seiten, um die Webparts für Administratoren und Benutzer an einem bekannten Speicherort zu hosten.

### <a name="disabling-telemetry-collection"></a>Deaktivieren der teleMetrie-Sammlung
Ein Teil dieser Lösung umfasst die anonymisierte Telemetrie-Verfolgung, die standardmäßig auf ein festgelegt ist. Wenn Sie eine manuelle Installation durchführen und die Telemetrie-Nachverfolgung deaktivieren möchten, ändern Sie `CustomlearningConfiguration.ps1` das Skript, um die Variable $optInTelemetry auf $false festzulegen.

Wenn Sie keine manuelle Installation durchführen und die Telemetrie-Verfolgung deaktivieren möchten, wurde ein separates `TelemetryOptOut.ps1` Skript hinzugefügt, das beim Ausführen die Telemetrie-Nachverfolgung deaktiviert.

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>ÜberPrüfen der erfolgreichen Ausführung und Initialisieren der CustomConfig-Liste

Nachdem das PowerShell-Skript erfolgreich ausgeführt wurde, navigieren Sie zur Website, initialisieren das **CustomConfig** -Listenelement, das benutzerdefiniertes lernen für die erste Verwendung festlegt, und überprüfen, ob die Website funktioniert.

1. Wechseln Sie zu `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`. Öffnen von **CustomLearningAdmin. aspx** initialisiert das **CustomConfig** -Listenelement, das benutzerdefiniertes lernen für die erste Verwendung festlegt. Es sollte eine Seite angezeigt werden, die wie folgt aussieht:

![CG-adminapppage. png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Hinzufügen von Besitzern zur Website
Als MandantenAdministrator ist es unwahrscheinlich, dass Sie die Website anpassen, daher müssen Sie der Website einige Besitzer zuweisen. Besitzer verfügen über Administratorrechte für die Website, damit Sie Website Seiten ändern und die Website neu bebranden können. Außerdem können Sie Inhalte, die über das benutzerdefinierte Lern Webpart übermittelt werden, ausblenden und anzeigen. Darüber hinaus haben Sie die Möglichkeit, benutzerdefinierte Wiedergabelisten zu erstellen und Sie benutzerdefinierten Unterkategorien zuzuweisen.  

1. Klicken Sie im Menü SharePoint- **Einstellungen** auf **Websiteberechtigungen**.
2. Klicken Sie auf **Erweiterte Berechtigungseinstellungen**.
3. Klicken Sie auf **benutzerdefiniertes lernen für Office 365-Besitzer**.
4. Klicken Sie auf **neue** > **Benutzer zu dieser Gruppe hinzufügen**, und fügen Sie dann die Personen hinzu, die Besitzer sein sollen. 
5. Fügen Sie einen Link hinzu, um die Website in der Freigabenachricht zu [Durchsuchen](https://docs.microsoft.com/en-us/Office365/CustomLearning/custom_explore) , und klicken Sie dann auf **Freigeben**.

### <a name="next-steps"></a>Weitere Schritte
- [Passen](custom_overview.md) Sie die Schulungsumgebung für Ihre Organisation an.

