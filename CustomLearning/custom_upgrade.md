---
author: pkrebs
ms.author: pkrebs
title: Benutzerdefiniertes Lern Upgrade
ms.date: 02/10/2019
description: Benutzerdefiniertes Learning for Office 365 Manual-Webpart-Setup
ms.openlocfilehash: 107db753c5b235cccb48b5a2f4d036f7de9d5639
ms.sourcegitcommit: c8c2bed48a1d3216618e7be368dda2855d1a0c14
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/28/2019
ms.locfileid: "30936395"
---
# <a name="manual-upgrade-for-custom-learning"></a>Manuelles Upgrade für benutzerdefiniertes lernen

Benutzerdefiniertes lernen für Office 365 bietet einen manuellen Aktualisierungsprozess für Organisationen, die an früheren Piloten teilgenommen haben. Mit dem Upgradeprozess können Organisationen weiterhin Ihre aktuelle benutzerdefinierte Lernwebsite und ein Upgrade verwenden, indem Sie dem SharePoint-App-Katalog das neue, Erweiterte benutzerdefinierte Lern Webpart hinzufügen und dann ein PowerShell-Skript ausführen. Im folgenden finden Sie eine Übersicht über den Upgradeprozess: 

- Überprüfen, ob die Person, die für das Hochladen des neuen Webparts verantwortlich ist und das PowerShell-Skript ausführt, über die erforderlichen Berechtigungen verfügt
- Hochladen des Webparts, customlearning. sppkg-Datei, in Ihren Office 365-Mandanten-App-Katalog
- Führen Sie ein PowerShell-Skript aus, das Ihren Mandanten mit den entsprechenden Artefakten konfiguriert, die für das benutzerdefinierte Lernen erforderlich sind.
- Navigieren Sie zur Seite CustomLearningAdmin. aspx in der benutzerdefinierten Lernsite, um die benutzerdefinierte Ccontent-Konfiguration zu initialisieren.

## <a name="prerequisites"></a>Voraussetzungen
Um ein erfolgreiches Upgrade von benutzerdefiniertem lernen sicherzustellen, müssen die folgenden Voraussetzungen erfüllt sein. 

- Sie müssen einen Mandanten weiten App-Katalog eingerichtet haben. Wenn Sie keinen Mandanten-App-Katalog haben, finden Sie weitere Informationen unter [Einrichten Ihres Office 365](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) -Mandanten und folgen Sie dem Abschnitt Erstellen einer APP-katalogwebsite. 
- Wenn Ihr Mandanten weiter App-Katalog bereits bereitgestellt wurde, benötigen Sie Zugriff auf ein Konto, das über Rechte zum Hochladen eines Pakets darauf verfügt. Im Allgemeinen handelt es sich um ein Konto mit der SharePoint-Administrator Rolle. 
- Wenn ein Konto mit der Rolle des SharePoint-Administrators nicht funktioniert: Wechseln Sie zum SharePoint Admin Center, wählen Sie den App-Katalog aus, klicken Sie auf Besitzer, und melden Sie sich als einer der WebsitesammlungsAdministratoren an, oder fügen Sie das SharePoint-Administrator Konto hinzu, das für die Website fehlgeschlagen ist. Liste der SammlungsAdministratoren. 

## <a name="step-1---get-the-web-part-package-and-setup-script-from-github"></a>Schritt 1: Abrufen des Webpart-Pakets und des Setupskripts von GitHub
Im Rahmen des Setupvorgangs benötigen Sie das benutzerdefinierte Lern Webpart-Paket und das PowerShell-Setupskript.

1. Gehen Sie zum [benutzerdefinierten Lern-GitHub-Repository](https://github.com/pnp/custom-learning-office-365).
2. Klicken Sie auf **Klonen oder herunterladen**, und laden Sie dann **zip herunter**.   
3. Speichern Sie die **ZIP** -Datei an einem Speicherort auf dem lokalen Laufwerk.
4. Extrahieren Sie die **ZIP** -Datei auf Ihrem lokalen Laufwerk.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Schritt 2: Hochladen des Webparts in den Mandanten-App-Katalog
Zum Einrichten von benutzerdefiniertem lernen für Office 365 laden Sie die Datei customlearning. sppkg in den Mandanten weiten App-Katalog hoch und stellen Sie bereit. Weitere Informationen zum Hinzufügen einer App zum App-Katalog finden Sie unter [Verwenden des App-Katalogs, um benutzerdefinierte Geschäfts-Apps für Ihre SharePoint Online-Umgebung](https://docs.microsoft.com/en-us/sharepoint/use-app-catalog) zur Verfügung zu stellen.

1. Klicken Sie in Office 365 auf **Admin**.
2. Klicken Sie unter **Admin Centers**auf **SharePoint**.
3. Klicken Sie auf **apps** > -**App-Katalog** > **: Apps für SharePoint verteilen.**
4. Klicken Sie auf**Dateien** **hochladen** > .
5. Wählen Sie in dem Ordner, in dem Sie die ZIP-Datei gespeichert haben, den **Webpart** -Ordner aus, und wählen Sie dann **customlearning. sppkg aus.**
6. Klicken Sie auf **Bereitstellen**.

## <a name="step-3---add-the-custom-learning-for-office-365-app-to-the-site"></a>Schritt 3: Hinzufügen der benutzerdefinierten Learning for Office 365-App zur Website

1. Klicken Sie auf der SharePoint-Website auf das Menü System, und klicken Sie dann auf **app hinzufügen**. 
2. Klicken Sie unter **Ihre apps**auf **aus Ihrer Organisation**, und klicken Sie dann auf **benutzerdefiniertes lernen für Office 365**. 

## <a name="step-4---execute-powershell-configuration-script"></a>Schritt 4: PowerShell-Konfigurationsskript ausführen
Ein PowerShell- `CustomLearningConfiguration.ps1` Skript ist im ZIP-Download von GitHub enthalten. Sie müssen das Skript ausführen, um drei [Mandanten Eigenschaften](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/tenant-properties) zu erstellen, die die Lösung verwendet. Darüber hinaus erstellt das Skript zwei [einzelne Teile-App-Seiten](https://docs.microsoft.com/en-us/sharepoint/dev/spfx/web-parts/single-part-app-pages) in der Bibliothek für Website Seiten, um die Webparts für Administratoren und Benutzer an einem bekannten Speicherort zu hosten. Diese APP-Seiten sind:

- CustomAdministration. aspx
- CustomViewer. aspx

### <a name="to-run-the-powershell-script"></a>So führen Sie das PowerShell-Skript aus
- Führen Sie mithilfe von PowerShell `CustomLearningConfiguration.ps1` das Skript aus dem Webpart-Ordner aus dem GITHUB-zip aus. Bei erfolgreicher Ausführung werden drei Schlüssel-Wert-Paare und **BenutzerdefiniertEr Learning admin für Off...** im Befehlsfenster angezeigt.

### <a name="disabling-telemetry-collection"></a>Deaktivieren der teleMetrie-Sammlung
Benutzerdefiniertes lernen umfasst die anonymisierte Telemetrie-Verfolgung, die standardmäßig auf ein festgelegt ist. Wenn Sie die Telemetrie-Nachverfolgung deaktivieren möchten, ändern `CustomlearningConfiguration.ps1` Sie das Skript, `$optInTelemetry` um die `$false`Variable auf festzulegen.

## <a name="step-5---initialize-web-part-custom-configuration"></a>Schritt 5-Initialisieren der benutzerdefinierten WebPart-Konfiguration
Nachdem das PowerShell-Skript erfolgreich ausgeführt wurde, navigieren `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`Sie zu. Öffnen von **CustomLearningAdmin. aspx** initialisiert das **CustomConfig** -Listenelement, das benutzerdefiniertes lernen für die erste Verwendung festlegt. Es sollte eine Seite angezeigt werden, die wie folgt aussieht:

![CG-adminapppage. png](media/cg-adminapppage.png)

Das Upgrade ist jetzt abgeschlossen. Weitere Informationen zum Anpassen der benutzerdefinierten Lernsite und des Webparts für Ihre Umgebung finden Sie unter [Anpassen der Schulung](custom_overview.md).

## <a name="upgrade-instructions-for-site-owners"></a>Upgrade-Anweisungen für Websitebesitzer
Bei der benutzerdefinierten Schulung für Office 365 wurden verschiedene Verbesserungen am Webpart eingeführt. Das Arbeiten mit dem Webpart wird ausführlich im Abschnitt [Anpassen der Lernerfahrung](custom_overview.md) behandelt. Im Moment sollte der Websitebesitzer:  

- Stellen Sie sicher, dass das benutzerdefinierte Learning for Office 365-Webpart verfügbar ist. 
- Ersetzen des vorhandenen Webparts auf Seiten durch das neue Webpart
- Ersetzen Sie alle Links, die auf das alte Webpart verweisen.

### <a name="verify-the-custom-learning-for-office-365-web-part-is-available"></a>Sicherstellen, dass das benutzerdefinierte Learning for Office 365-Webpart verfügbar ist
1.  Klicken Sie auf der benutzerdefinierten Lernsite auf **Einstellungen**, und klicken Sie dann auf**Seite hinzufügen**.
2.  Klicken Sie **+** auf das Symbol auf der Seite, um ein Webpart hinzuzufügen, und wählen Sie dann das Webpart **für die benutzerdefinierte schulung für Office 365** aus. Die Seite sollte jetzt ähnlich wie die folgende Grafik aussehen:

![CG-adminapppage. png](media/cg-adminapppage.png)
 
### <a name="replace-the-old-web-part-with-the-new-web-part"></a>Ersetzen des alten Webparts durch das neue Webpart
Bevor Sie das benutzerdefinierte Lern Webpart ersetzen oder Änderungen an der Website vornehmen, empfehlen wir, dass Sie die Dokumentation zur [Lernumgebung anpassen](custom_overview.md) , wie Sie die Verwendung des neuen Webparts erläutert, lesen. 

Ersetzen Sie zum Aktualisieren der benutzerdefinierten Lernsite vorhandene Instanzen des Webparts durch das neue Webpart. Auch wenn wir nicht sicher sein können, wo das Webpart hinzugefügt wurde, war die Richtlinie für frühere Piloten, das Webpart auf den folgenden Seiten hinzuzufügen, um das Webpart auf diesen Seiten zu ersetzen:

- Get-started-with-Office-365. aspx
- Get-started-with-Microsoft-Teams. aspx
- Get-started-with-OneDrive. aspx
- Get-started-with-SharePoint. aspx

### <a name="replace-existing-links-to-the-web-part"></a>Ersetzen vorhandener Links in das Webpart
Durch die Verbesserungen am neuen Webpart wurde die Verknüpfung mit einer Wiedergabeliste geändert. Im Rahmen des Upgrades sollten Sie alle Links zu dem Webpart, einschließlich Menüelementen und Links auf der Homepage, ersetzen. Bevor Sie das benutzerdefinierte Lern Webpart ersetzen oder Änderungen an der Website vornehmen, empfehlen wir, dass Sie die Dokumentation zur [Lernumgebung anpassen](custom_overview.md) , wie Sie die Verwendung des neuen Webparts erläutert, lesen. 

## <a name="recreate-existing-playlists"></a>Erstellen vorhandener Wiedergabelisten 
Um sicherzustellen, dass Wiedergabelisten ordnungsgemäß ausgeführt werden, müssen alle Wiedergabelisten, die mit der früheren Version des Webparts erstellt wurden, wiederhergestellt werden. Erstellen Sie vor dem Löschen der Wiedergabelisten eine Liste der benutzerdefinierten Wiedergabelisten und der dazugehörigen Objekte, damit Sie Sie problemlos mit dem neuen benutzerdefinierten Lern Webpart wiederherstellen können. Erstellen Sie eine Kopie einer Wiedergabeliste, und löschen Sie Sie. Sie können das Feld JSONData verwenden, um eine Kopie des Inhalts einer Wiedergabeliste zu erstellen, bevor Sie Sie löschen. Dies erleichtert das Erstellen später.


1. Klicken Sie auf der benutzerdefinierten Lernsite auf **Einstellungen** > **Websiteinhalt**. 
2. Wählen Sie eine Wiedergabeliste aus, wählen Sie die Ellipsen aus, wählen Sie **Bearbeiten**aus, kopieren Sie dann den Inhalt des Felds **JSONData** , und speichern Sie ihn im Editor oder in einem separaten Dokument zu einem späteren Zeitpunkt. Wählen Sie **Abbrechen**aus.
3. Wählen Sie die Wiedergabeliste aus, wählen Sie die Ellipse aus, und wählen Sie dann **Löschen**aus.
4. Sie können nun die Wiedergabeliste mit dem neuen Webpart neu erstellen.
Anweisungen zur Verwendung des benutzerdefinierten Learning for Office 365-Webparts finden Sie unter [Customize the Learning Experience (custom_overview. MD).

### <a name="next-steps"></a>Weitere Schritte
- [Passen](custom_overview.md) Sie die Schulungsumgebung für Ihre Organisation an.

