---
author: pkrebs
ms.author: pkrebs
title: Manuelle Installation von Lernpfaden
ms.date: 02/18/2019
description: Manuelle Installation von Lernpfaden
ms.service: sharepoint online
ms.openlocfilehash: a9ae97bbafcc82c54251cae9a0ad658b7a0c16f4
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/23/2020
ms.locfileid: "48234667"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>Manuelles Installieren und Konfigurieren von benutzerdefiniertem lernen für Office 365

Das Microsoft Custom Learning-Webpart wird mithilfe der [SharePoint-Framework](https://docs.microsoft.com/sharepoint/dev/spfx/sharepoint-framework-overview) -Version 1.7.1 erstellt.

Zum manuellen Installieren und Konfigurieren des Webparts und der Websitesammlung müssen Sie die folgenden Schritte ausführen:

1. Überprüfen Sie, ob Sie alle Voraussetzungen erfüllt haben.
1. Installieren Sie die Datei customlearning. sppkg in Ihrem Office 365 Mandanten-App-Katalog.
1. Stellen Sie eine moderne Kommunikationswebsite zur Verfügung, die als benutzerdefiniertes lernen für Office 365 Home-Website fungiert.
1. Führen Sie ein PowerShell-Skript aus, mit dem Ihr Mandant mit den entsprechenden Artefakten konfiguriert wird, von denen benutzerdefinierte Lernprozesse abhängig sind.
1. Navigieren Sie zur Seite CustomLearningAdmin. aspx, um das Admin-Webpart zu laden, um die benutzerdefinierte Inhalts Konfiguration zu initialisieren.

## <a name="prerequisites"></a>Voraussetzungen

Sie müssen den Mandanten weiten App-Katalog eingerichtet und konfiguriert haben. Weitere Informationen finden Sie unter [Einrichten des Office 365 Mandanten](https://docs.microsoft.com/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) und dem Abschnitt Erstellen der APP-katalogwebsite. Wenn Ihr Mandanten weiter App-Katalog bereits bereitgestellt wurde, benötigen Sie Zugriff auf ein Konto, das über Rechte zum Hochladen eines Pakets verfügt, damit dieser Setupvorgang abgeschlossen wird. Im Allgemeinen handelt es sich hierbei um ein Konto mit der SharePoint-Administratorrolle. Wenn ein Konto mit dieser Rolle nicht funktioniert, wechseln Sie zum SharePoint Admin Center, suchen Sie die Websitesammlungsadministratoren für die APP-Katalog-Websitesammlung, und melden Sie sich entweder als Websitesammlungsadministrator an, oder fügen Sie das SharePoint-Administratorkonto hinzu, das den Websitesammlungsadministratoren nicht erfolgreich war. Sie benötigen auch Zugriff auf ein Konto, bei dem es sich um einen SharePoint-mandantenadministrator handelt.

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>Hochladen des Webparts in den Mandanten-App-Katalog

Zum Einrichten von benutzerdefiniertem lernen für Office 365 laden Sie die Datei customlearning. sppkg in den Mandanten weiten App-Katalog hoch und stellen Sie bereit. Ausführliche Anweisungen zum Hinzufügen einer App zum App-Katalog finden Sie unter [Verwenden des App-Katalogs, um benutzerdefinierte Business-Apps für Ihre SharePoint Online Umgebung zur Verfügung zu stellen](https://docs.microsoft.com/sharepoint/use-app-catalog) .

## <a name="provisionidentify-modern-communication-site"></a>Bereitstellungs-und Identifikations Website für moderne Kommunikation

Identifizieren Sie entweder eine vorhandene SharePoint-Kommunikationswebsite, oder stellen Sie eine neue in Ihrem SharePoint Online Mandanten zur Verfügung. Weitere Informationen zum Einrichten einer Kommunikationswebsite finden Sie unter [Create a Communication Site in SharePoint Online](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) und folgen den Schritten zum Erstellen einer Kommunikationswebsite.

## <a name="set-permissions-for-the-site"></a>Festlegen von Berechtigungen für die Website

Sie sollten alle Personen hinzufügen, die Inhalte in der Gruppe "Besucher" anzeigen können, und alle Benutzer, die in der Lage sein sollen, benutzerdefinierte Wiedergabelisten für die Mitgliedergruppe zu verwalten. So konfigurieren Sie die Website für benutzerdefiniertes Lernen beim ersten Mal muss es sich bei dem Benutzer um einen Websitesammlungsadministrator oder einen Teil der Gruppe "Besitzer" handeln.

Fügen Sie der Websitesammlung benutzerdefiniertes lernen für Office 365-APP hinzu.

## <a name="execute-powershell-configuration-script"></a>Ausführen des PowerShell-Konfigurationsskripts

Ein PowerShell `CustomLearningConfiguration.ps1` -Skript ist enthalten, das Sie ausführen müssen, um drei [Mandanten Eigenschaften](https://docs.microsoft.com/sharepoint/dev/spfx/tenant-properties) zu erstellen, die von der Lösung verwendet werden. Darüber hinaus erstellt das Skript zwei [einzelne Teile-App-Seiten](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/single-part-app-pages) in der Bibliothek Website Seiten, um die Administrator-und Benutzer Webparts an einem bekannten Speicherort zu hosten.

### <a name="disabling-telemetry-collection"></a>Deaktivieren der Telemetrie-Sammlung

Ein Teil dieser Lösung umfasst die anonymisierte Telemetrie-Überwachung Opt in, die standardmäßig auf ein festgelegt ist. Wenn Sie eine manuelle Installation durchführen und die Telemetrie-Verfolgung deaktivieren möchten, ändern Sie das `CustomlearningConfiguration.ps1` Skript, um die $optInTelemetry Variable auf $false festzulegen.

Wenn Sie keine manuelle Installation durchführen und die Telemetrie-Verfolgung deaktivieren möchten, wurde ein separates Skript `TelemetryOptOut.ps1` hinzugefügt, das bei Ausführung die Telemetrie-Nachverfolgung deaktiviert.

## <a name="initialize-web-part-custom-configuration"></a>Benutzerdefinierte Webparts-Konfiguration initialisieren

Nachdem das PowerShell-Skript erfolgreich ausgeführt wurde, navigieren Sie zu `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` . Dadurch wird das CustomConfig-Listenelement initialisiert, mit dem benutzerdefiniertes lernen für die erste Verwendung eingerichtet wird.

Die Konfiguration ist nun abgeschlossen, und Sie können mit der Verwendung von benutzerdefiniertem lernen für Office 365 fortfahren. Weitere Informationen finden Sie in der Benutzerdokumentation.