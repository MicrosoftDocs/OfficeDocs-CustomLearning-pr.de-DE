---
author: pkrebs
ms.author: pkrebs
title: Manuelles Installieren von Lernpfaden
ms.date: 02/18/2019
manager: bpardi
description: Manuelles Installieren von Lernpfaden
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: 6f106b569602730f16fc2b6f8a09fa44667e32e1
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575970"
---
# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>Manuelles Installieren und Konfigurieren von Custom Learning für Office 365

Das Microsoft Custom Learning Web [](/sharepoint/dev/spfx/sharepoint-framework-overview) Part wird mithilfe der SharePoint-Framework Version 1.7.1 erstellt.

Um das Webteil und die Websitesammlung manuell zu installieren und zu konfigurieren, müssen Sie die folgenden Schritte ausführen:

1. Überprüfen Sie, ob alle Voraussetzungen erfüllt sind.
1. Installieren Sie die Datei customlearning.sppkg in Office 365 Mandanten-App-Katalog.
1. Bereitstellen/Identifizieren einer modernen Kommunikationswebsite, die als Benutzerdefiniertes Lernen für die Office 365 fungieren soll.
1. Führen Sie ein PowerShell-Skript aus, das Ihren Mandanten mit den entsprechenden Artefakten konfiguriert, von dem benutzerdefiniertes Lernen abhängt.
1. Navigieren Sie zur Websiteseite CustomLearningAdmin.aspx, um das Administratorwebteil zu laden, um die benutzerdefinierte Inhaltskonfiguration zu initialisieren.

## <a name="prerequisites"></a>Voraussetzungen

Sie müssen den mandantenweiten App-Katalog eingerichtet und konfiguriert haben. Weitere Informationen finden Sie unter Einrichten [Office 365 Mandanten,](/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) und folgen Sie dem Abschnitt Erstellen einer App-Katalogwebsite. Wenn Ihr mandantenweiter App-Katalog bereits bereitgestellt wurde, benötigen Sie Zugriff auf ein Konto, das Über die Rechte zum Hochladen eines Pakets darauf verfügt, um diesen Setupvorgang abzuschließen. Im Allgemeinen verfügt dieses Konto SharePoint Administratorrolle. Wenn ein Konto mit dieser Rolle nicht funktioniert, wechseln Sie zum SharePoint Admin Center, suchen Sie die Websitesammlungsadministratoren für die Websitesammlung des App-Katalogs, und melden Sie sich entweder als einer der Websitesammlungsadministratoren an, oder fügen Sie das SharePoint-Administratorkonto hinzu, das den Websitesammlungsadministratoren nicht möglich war. Außerdem benötigen Sie Zugriff auf ein Konto, das ein SharePoint ist.

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>Hochladen web part to the Tenant App Catalog

Zum Einrichten von Custom Learning für Office 365 laden Sie die Datei customlearning.sppkg in den mandantenweiten App-Katalog hoch und stellen sie zur Bereitstellung. Ausführliche Anweisungen zum Hinzufügen einer App zum App-Katalog finden Sie unter Use the App Catalog to [make custom business apps available for your SharePoint Online](/sharepoint/use-app-catalog) environment.

## <a name="provisionidentify-modern-communication-site"></a>Bereitstellen/Identifizieren einer modernen Kommunikationswebsite

Identifizieren Sie entweder eine vorhandene SharePoint Oder stellen Sie eine neue in Ihrem SharePoint Online-Mandanten zur Verfügung. Weitere Informationen zum Bereitstellen einer Kommunikationswebsite finden Sie unter Erstellen einer Kommunikationswebsite [in SharePoint Online,](https://support.office.com/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) und führen Sie die Schritte zum Erstellen einer Kommunikationswebsite aus.

## <a name="set-permissions-for-the-site"></a>Festlegen von Berechtigungen für die Website

Sie möchten alle Personen hinzufügen, die Inhalte der Gruppe Besucher anzeigen können sollen, sowie alle Benutzer, die benutzerdefinierte Wiedergabelisten der Gruppe Mitglieder verwalten können sollten. Um die Website für benutzerdefiniertes Lernen zu konfigurieren, muss der Benutzer zum ersten Mal entweder Ein Websitesammlungsadministrator oder Teil der Gruppe Besitzer sein.

Fügen Sie der Websitesammlung Office 365 Benutzerdefiniertes Lernen für die App hinzu.

## <a name="execute-powershell-configuration-script"></a>Ausführen des PowerShell-Konfigurationsskripts

Ein PowerShell-Skript ist enthalten, das Sie ausführen müssen, um drei Mandanteneigenschaften zu erstellen, die `CustomLearningConfiguration.ps1` von der Lösung verwendet werden. [](/sharepoint/dev/spfx/tenant-properties) Darüber hinaus erstellt das Skript zwei [einzelne Teil-App-Seiten](/sharepoint/dev/spfx/web-parts/single-part-app-pages) in der Websiteseitenbibliothek, um die Administrator- und Benutzerwebparts an einem bekannten Speicherort zu hosten.

### <a name="disabling-telemetry-collection"></a>Deaktivieren der Telemetriesammlung

Teil dieser Lösung ist die anonymisierte Telemetrieverfolgung, die standardmäßig auf aktiviert festgelegt ist. Wenn Sie eine manuelle Installation durchführen und die Telemetrieverfolgung deaktivieren möchten, ändern Sie das Skript so, dass die variable $optInTelemetry auf `CustomlearningConfiguration.ps1` $false.

Wenn Sie keine manuelle Installation durchführen und die Telemetrieverfolgung deaktivieren möchten, wurde ein separates Skript enthalten, das bei der Ausführung die Telemetrieverfolgung `TelemetryOptOut.ps1` deaktiviert.

## <a name="initialize-web-part-custom-configuration"></a>Initialisieren der benutzerdefinierten Web part-Konfiguration

Navigieren Sie nach der erfolgreichen Ausführung des PowerShell-Skripts zu `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx` . Dadurch wird das Listenelement CustomConfig initialisiert, das benutzerdefiniertes Lernen für die erste Verwendung eingerichtet hat.

Die Konfiguration ist nun abgeschlossen, und Sie können mit der Verwendung von Custom Learning for Office 365. Weitere Informationen finden Sie in der Benutzerdokumentation.
