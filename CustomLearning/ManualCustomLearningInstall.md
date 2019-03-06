# <a name="manually-installing-and-configuring-custom-learning-for-office-365"></a>Manuelles Installieren und Konfigurieren von benutzerdefiniertem Learning für Office 365

Das Microsoft Custom Learning-Webpart wird mit der [SharePoint Framework](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/sharepoint-framework-overview) -Version 1.7.1 erstellt.

Um das Webpart und die Websitesammlung manuell zu installieren und zu konfigurieren, müssen Sie die folgenden Schritte ausführen:

1. Überprüfen Sie, ob alle Voraussetzungen erfüllt sind.
1. Installieren Sie die Datei customlearning. sppkg im Office 365-Mandanten-App-Katalog.
1. Stellen Sie eine moderne Kommunikationswebsite zur Verfügung, die als benutzerdefiniertes Learning für Office 365-Homepage dient.
1. Führen Sie ein PowerShell-Skript aus, das den Mandanten mit den entsprechenden Artefakten konfiguriert, von denen die benutzerdefinierte Schulung abhängig ist.
1. Navigieren Sie zur Seite CustomLearningAdmin. aspx, um das Admin-Webpart zu laden, um die benutzerdefinierte Inhalts Konfiguration zu initialisieren.

## <a name="prerequisites"></a>Voraussetzungen

Sie müssen den Mandanten weiten App-Katalog eingerichtet und konfiguriert haben. Weitere Informationen finden Sie unter [Einrichten Ihres Office 365](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) -Mandanten und folgen Sie dem Abschnitt Erstellen einer APP-katalogwebsite. Wenn Ihr Mandanten weiter App-Katalog bereits bereitgestellt wurde, benötigen Sie Zugriff auf ein Konto, das über die Berechtigung zum Hochladen eines Pakets zum Ausführen dieses Setupvorgangs verfügt. Im Allgemeinen handelt es sich um ein Konto mit der SharePoint-Administratorrolle. Wenn ein Konto mit dieser Rolle nicht funktioniert, wechseln Sie zum SharePoint Admin Center, suchen Sie die WebsitesammlungsAdministratoren für die Websitesammlung des App-Katalogs, und melden Sie sich als einer der WebsitesammlungsAdministratoren an, oder fügen Sie das SharePoint-Administratorkonto hinzu. , die den WebsitesammlungsAdministratoren nicht gelungen sind. Sie benötigen außerdem Zugriff auf ein Konto, das ein SharePoint-MandantenAdministrator ist.

## <a name="upload-the-web-part-to-the-tenant-app-catalog"></a>Hochladen des Webparts in den Mandanten-App-Katalog

Zum Einrichten von benutzerdefiniertem lernen für Office 365 laden Sie die Datei customlearning. sppkg in den Mandanten weiten App-Katalog hoch und stellen Sie bereit. Weitere Informationen zum Hinzufügen einer App zum App-Katalog finden Sie unter [Verwenden des App-Katalogs, um benutzerdefinierte Geschäfts-Apps für Ihre SharePoint Online-Umgebung](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) zur Verfügung zu stellen.

## <a name="provisionidentify-modern-communication-site"></a>Bestimmung/Identifizierung der modernen Kommunikationswebsite

Identifizieren Sie eine vorhandene SharePoint-Kommunikationswebsite, oder stellen Sie eine neue in Ihrem SharePoint Online-Mandanten ein. Weitere Informationen zum Einrichten einer Kommunikationswebsite finden Sie unter [Erstellen einer Kommunikationswebsite in SharePoint Online](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) und führen Sie die Schritte zum Erstellen einer Kommunikationswebsite aus.

## <a name="set-permissions-for-the-site"></a>Festlegen von Berechtigungen für die Website

Sie möchten alle Benutzer hinzufügen, die Inhalte für die Gruppe "Besucher" anzeigen können sollen, und alle Personen, die in der Lage sein sollen, angepasste Wiedergabelisten für die Gruppe Mitglieder zu verwalten. So konfigurieren Sie die Website für das benutzerdefinierte lernen, wenn der Benutzer zum ersten Mal ein Websitesammlungsadministrator oder ein Teil der Gruppe Besitzer sein muss.

Fügen Sie der Websitesammlung benutzerdefinierte Learning for Office 365-APP hinzu.

## <a name="execute-powershell-configuration-script"></a>PowerShell-Konfigurationsskript ausführen

Ein PowerShell- `CustomLearningConfiguration.ps1` Skript ist enthalten, das Sie ausführen müssen, um drei [Mandanten Eigenschaften](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) zu erstellen, die die Lösung verwendet. Darüber hinaus erstellt das Skript zwei [einzelne Teile-App-Seiten](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) in der Bibliothek für Website Seiten, um die Webparts für Administratoren und Benutzer an einem bekannten Speicherort zu hosten.

### <a name="disabling-telemetry-collection"></a>Deaktivieren der teleMetrie-Sammlung

Ein Teil dieser Lösung umfasst die anonymisierte Telemetrie-Verfolgung, die standardmäßig auf ein festgelegt ist. Wenn Sie eine manuelle Installation durchführen und die Telemetrie-Nachverfolgung deaktivieren möchten, ändern Sie `CustomlearningConfiguration.ps1` das Skript, um die Variable $optInTelemetry auf $false festzulegen.

Wenn Sie keine manuelle Installation durchführen und die Telemetrie-Verfolgung deaktivieren möchten, wurde ein separates `TelemetryOptOut.ps1` Skript hinzugefügt, das beim Ausführen die Telemetrie-Nachverfolgung deaktiviert.

## <a name="initialize-web-part-custom-configuration"></a>Initialisieren der benutzerdefinierten Konfiguration des Webparts

Nachdem das PowerShell-Skript erfolgreich ausgeführt wurde, navigieren `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`Sie zu. Dadurch wird das CustomConfig-Listenelement initialisiert, das benutzerdefiniertes lernen für die erste Verwendung festlegt.

Die Konfiguration ist nun abgeschlossen, und Sie können mit der Verwendung von benutzerdefiniertem lernen für Office 365 fortfahren. Weitere Informationen finden Sie in der Benutzerdokumentation.