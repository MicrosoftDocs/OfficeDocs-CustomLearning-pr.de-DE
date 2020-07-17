---
author: pkrebs
ms.author: pkrebs
title: Manuelle Einrichtung von Lernpfaden
ms.date: 07/06/2020
description: Manuelle Einrichtung von Microsoft 365 Lernpfaden
ms.openlocfilehash: f980722fed48b5f92fb595cf8286604b3fa6d409
ms.sourcegitcommit: ba0cddd12dd8687ec4b97c26174fdda09de83b05
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 07/06/2020
ms.locfileid: "45043267"
---
# <a name="learning-pathways-manual-setup"></a>Manuelle Einrichtung von Lernpfaden

Microsoft 365-Lern Pfade bieten eine manuelle Einrichtung für Organisationen, die Unterstützung für eines der folgenden Szenarien benötigen: 

- Ihre Organisation verfügt über eine etablierte SharePoint Online moderne Kommunikationswebsite, die der Schulung gewidmet ist, und Sie möchten dieser Website Lern Pfade hinzufügen. In diesem Szenario wurde das Lern Pfad-Webpart nicht auf der Website eingerichtet.

- Sie möchten Lern Pfade für mehrsprachige Unterstützung in einer der SharePoint-Kommunikationswebsites Ihrer Organisation installieren. Die Website hat eine Standardsprache, die nicht Englisch ist und eine der Sprachen ist, die von Lernpfaden unterstützt werden. Hier sind die Sprachen, die von Lernpfaden unterstützt werden:

- English
- Chinesisch (vereinfacht)
- Französisch
- Deutsch
- Italienisch (Italien)
- Japanisch (Japan)
- Portugiesisch (Brasilien)
- Russisch (Russisch)
- Spanisch

Das manuelle Einrichten von Lernpfaden erfordert Erfahrung in der Arbeit mit Windows PowerShell und der SharePoint Online-Verwaltungsshell. Im folgenden finden Sie eine Übersicht über die Schritte für das manuelle Einrichten von Lernpfaden: 

- Überprüfen Sie, ob Sie alle Voraussetzungen erfüllt haben.
- Überprüfen Sie die Standardspracheinstellungen für Ihre Website. Wenn OK, fahren Sie mit manueller Installation fort. Wenn Sie eine andere Standardspracheinstellung benötigen, müssen Sie eine neue Website erstellen. 
- Installieren Sie die Datei customlearning. sppkg in Ihrem SharePoint-Mandanten-App-Katalog.
- Stellen Sie eine moderne Kommunikationswebsite zur Verfügung, die Sie als Microsoft 365-Lern Pfade als Startseite fungieren möchten.
- Führen Sie ein PowerShell-Skript aus, mit dem Ihr Mandant mit den Artefakten konfiguriert wird, von denen Lern Pfade abhängen.
- Navigieren Sie zur Seite CustomLearningAdmin. aspx, um das Admin-Webpart zu laden, um die Konfiguration mit benutzerdefiniertem Inhalt zu initialisieren.

## <a name="prerequisites"></a>Voraussetzungen
Um eine erfolgreiche manuelle Einrichtung des Webparts für Lern Pfade sicherzustellen, müssen die folgenden Voraussetzungen erfüllt sein. 

- Sie müssen den Mandanten weiten App-Katalog eingerichtet und konfiguriert haben. Weitere Informationen finden Sie unter [Einrichten des Office 365 Mandanten](https://docs.microsoft.com/sharepoint/dev/spfx/set-up-your-developer-tenant#create-app-catalog-site) und im Abschnitt "Erstellen eines App-Katalogs" auf der Website. 
- Wenn Ihr Mandanten weiter App-Katalog bereits bereitgestellt wurde, benötigen Sie Zugriff auf ein Konto, das über Rechte zum Hochladen eines Pakets verfügt. Im allgemeinen verfügt dieses Konto über eine SharePoint-Administratorrolle. 
- Wenn ein Konto mit dieser Rolle nicht funktioniert, wechseln Sie zum SharePoint Admin Center, und suchen Sie die Websitesammlungsadministratoren für die APP-Katalog-Websitesammlung, und melden Sie sich als einer der Websitesammlungsadministratoren an, oder fügen Sie das SharePoint-Administratorkonto hinzu, das den Websitesammlungsadministratoren nicht erfolgreich war. 
- Sie benötigen auch Zugriff auf ein Konto, bei dem es sich um einen SharePoint-mandantenadministrator handelt.

## <a name="step-1---check-your-language-settings"></a>Schritt 1: Überprüfen der Spracheinstellungen
Überprüfen Sie im ersten Schritt des manuellen Installationsprozesses die Spracheinstellungen Ihrer Website. Die folgenden Optionen sind möglich:

### <a name="option-1---you-dont-want-multilingual-support"></a>Option 1 – Sie möchten keine mehrsprachige Unterstützung
Wenn Sie keine mehrsprachige Unterstützung für Ihre Website wünschen, stellen Sie sicher, dass Sie deaktiviert ist.
1.  Wählen Sie auf der SharePoint-Kommunikationswebsite **Einstellungen**  >  **Website Informationen**  >  alle Spracheinstellungen für**Websiteeinstellungen anzeigen**aus  >  **Language settings**. 
2.  Legen Sie **fest, dass**die Option **Seiten und Nachrichten in mehrere Sprachen übersetzt aktiviert werden** soll.
3.  Klicken Sie auf **Speichern**. 
4.  Fahren Sie mit Schritt 2 fort.

## <a name="option-2---you-want-multilingual-support-and-youre-ok-with-the-default-language"></a>Option 2-Sie möchten mehrsprachige Unterstützung und sind mit der Standardsprache in Ordnung
Eine SharePoint-Kommunikationswebsite verfügt über eine Standardsprache. Die Standardsprache bestimmt die Sprache, in der Sie Lern Pfade anzeigen, einschließlich der Verwaltungsseite für Lern Pfade. Die Einstellung für die Standardsprache wird festgelegt, wenn die Website erstmalig erstellt wird, und kann danach nicht mehr geändert werden. Stellen Sie sicher, dass Sie mit der Standardsprache der Zielwebsite in Ordnung sind, bevor Sie mit dem manuellen Setup fortfahren.

1.  Wählen Sie auf der SharePoint-Kommunikationswebsite **Einstellungen**  >  **Website Informationen**  >  alle Spracheinstellungen für**Websiteeinstellungen anzeigen**aus  >  **Language settings**. 
2.  Legen Sie die Option **Seiten und Nachrichten aktivieren in mehrere Sprachen übersetzt** als **auf ein**fest.
    - Wenn Sie mit der Sprache, die oben in der Liste angezeigt wird **, in Ordnung sind, können**Sie weitere Sprachen hinzufügen und dann auf **Speichern**klicken. Fahren Sie mit Schritt 2 fort.
    - Wenn Sie eine andere Standardsprache als die für die Website ausgewählten auswählen möchten, müssen Sie eine neue SharePoint-Kommunikationswebsite mit der gewünschten Sprache erstellen. Fahren Sie mit Option 3 fort. 

## <a name="option-3---you-want-multilingual-support-but-want-a-different-default-language-for-the-site"></a>Option #3-Sie möchten mehrsprachige Unterstützung, möchten jedoch eine andere Standardsprache für die Website verwenden
Mit dieser Option erstellen Sie eine neue SharePoint Online Kommunikationswebsite mit der gewünschten Standardsprache und legen dann die Spracheinstellungen für die Website fest. 
1.  Informationen zum Erstellen einer neuen SharePoint-Kommunikationswebsite finden Sie unter [Create a Communication Site in SharePoint Online](https://support.microsoft.com/office/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb). Achten Sie beim Erstellen der Website darauf, die Sprache auf die Standardsprache festzulegen, die Sie für Lern Pfade benötigen. 
2. Wählen Sie auf der von Ihnen erstellten Website **Einstellungen**  >  **Website Informationen**  >  **alle**  >  **Spracheinstellungen**für Websiteeinstellungen anzeigen aus. 
2.  Legen Sie die Option **Seiten und Nachrichten aktivieren in mehrere Sprachen übersetzt** als **auf ein**fest.
3. Fügen Sie bei Bedarf weitere Sprachen hinzu, und klicken Sie dann auf **Speichern**. 
4. Fahren Sie mit Schritt 2 fort. 

>! Hinweis Wenn Sie benutzerdefinierten Inhalt von einer Website zu einer neu erstellten Website migrieren müssen, lesen Sie den Abschnitt "benutzerdefinierten Inhalt migrieren" weiter unten in diesem Dokument. 

## <a name="step-2---get-the-web-part-package-and-setup-script-from-github"></a>Schritt 2: Abrufen des Webpart-Pakets und des Setupskripts von GitHub
Im Rahmen des Setupprozesses benötigen Sie das Microsoft 365 Learning-Pfad-Webpart-Paket und das PowerShell-Setupskript.

- Wechseln Sie zum [GitHub-Repository für Lern Pfade](https://github.com/pnp/custom-learning-office-365).
- Klicken Sie auf **herunterladen** , um das Webparts-Paket und das Skript auf einem lokalen Laufwerk zu speichern. Sie verwenden das Skript und das Webpart-Paket in späteren Schritten dieses Prozesses.

## <a name="step-2---upload-the-web-part-to-the-tenant-app-catalog"></a>Schritt 2: Hochladen des Webparts in den Mandanten-App-Katalog
Um Microsoft 365-Lern Pfade einzurichten, laden Sie die Datei customlearning. sppkg in den Mandanten weiten App-Katalog hoch und stellen Sie bereit. Ausführliche Anweisungen zum Hinzufügen einer App zum App-Katalog finden Sie unter [Verwenden des App-Katalogs, um benutzerdefinierte Business-Apps für Ihre SharePoint Online Umgebung zur Verfügung zu stellen](https://docs.microsoft.com/sharepoint/use-app-catalog) .

## <a name="step-3---provisionidentify-a-modern-communication-site"></a>Schritt 3 – Bereitstellung/Identifizierung einer modernen Kommunikationswebsite
Identifizieren Sie entweder eine vorhandene SharePoint-Kommunikationswebsite, oder stellen Sie eine neue in Ihrem SharePoint Online Mandanten zur Verfügung. Weitere Informationen zum Einrichten einer Kommunikationswebsite finden Sie unter [Create a Communication Site in SharePoint Online](https://support.office.com/en-us/article/create-a-communication-site-in-sharepoint-online-7fb44b20-a72f-4d2c-9173-fc8f59ba50eb) und folgen den Schritten zum Erstellen einer Kommunikationswebsite.

## <a name="step-4---add-the-microsoft-365-learning-pathways-app-to-the-site"></a>Schritt 4 – Hinzufügen der App "Microsoft 365 Learning Pfads" zur Website

1. Klicken Sie auf der SharePoint-Website auf das Menü System, und klicken Sie dann auf **app hinzufügen**. 
2. Klicken Sie unter **Ihre apps**auf **aus Ihrer Organisation**, und klicken Sie dann auf **Lern Pfade für Office 365**. 

## <a name="step-5---set-permissions-for-the-site"></a>Schritt 5 – Festlegen von Berechtigungen für die Website
Stellen Sie sicher, dass die folgenden Berechtigungen für die Website festgelegt sind:
- **Website Sammlungs Administrator oder Teil der Gruppe Besitzer** – erforderliche Berechtigungen zum Initialisieren des CustomConfig-Listenelements, das Lern Pfade für die erste Verwendung einrichtet. 
- **Mitgliedergruppe** – Berechtigungen, die für die Verwaltung von Lernpfaden erforderlich sind, einschließlich ausblenden und Anzeigen von Inhalten und Verwalten benutzerdefinierter Wiedergabelisten
- **Besuchergruppe** – für die Anzeige von Websiteinhalten sind Berechtigungen erforderlich. 

## <a name="step-6--execute-powershell-configuration-script"></a>Schritt 6-Ausführen des PowerShell-Konfigurationsskripts
Ein PowerShell `CustomLearningConfiguration.ps1` -Skript ist enthalten, das Sie ausführen müssen, um drei [Mandanten Eigenschaften](https://docs.microsoft.com/sharepoint/dev/spfx/tenant-properties) zu erstellen, die von der Lösung verwendet werden. Darüber hinaus erstellt das Skript zwei [einzelne Teile-App-Seiten](https://docs.microsoft.com/sharepoint/dev/spfx/web-parts/single-part-app-pages) in der Bibliothek Website Seiten, um die Administrator-und Benutzer Webparts an einem bekannten Speicherort zu hosten.

1. Wenn Sie die SharePoint Online Management-Shell noch nicht heruntergeladen haben, laden Sie Sie jetzt herunter. Weitere Informationen finden Sie unter [SharePoint Online Management Shell Download](https://go.microsoft.com/fwlink/p/?LinkId=255251).
2. Möglicherweise müssen Sie eine PowerShell-Ausführungsrichtlinie festlegen, um das Skript auszuführen. Weitere Informationen finden Sie unter [Informationen zu Ausführungsrichtlinien](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).
3. Führen Sie das `CustomLearningConfiguration.ps1` Skript aus. Zusätzlich zu den Anmeldeinformationen für den mandantenadministrator werden Sie vom Skript aufgefordert, ihren Mandantennamen und den Websitenamen einzugeben. In Anbetracht des folgenden Beispiels für Ihre Website-URL `https://contoso.sharepoint.com/sites/O365CL` `contoso` ist der Name des Mandanten und `O365CL` der Name der Website. 

### <a name="disabling-telemetry-collection"></a>Deaktivieren der Telemetrie-Sammlung
Ein Teil dieser Lösung umfasst die anonymisierte Telemetrie-Überwachung Opt in, die standardmäßig auf ein festgelegt ist. Wenn Sie eine manuelle Installation durchführen und die Telemetrie-Verfolgung deaktivieren möchten, ändern Sie das `CustomlearningConfiguration.ps1` Skript so, dass die $optInTelemetry Variable auf $false und das Skript ausgeführt wird.

## <a name="validate-provisioning-success-and-initialize-the-customconfig-list"></a>Überprüfen des Erfolgs der Vorstellung und Initialisieren der CustomConfig-Liste

Nachdem das PowerShell-Skript erfolgreich ausgeführt wurde, navigieren Sie zur Website, initialisieren das **CustomConfig** -Listenelement, das Lern Pfade für die erste Verwendung einrichtet, und überprüfen, ob die Website funktioniert.

- Navigieren Sie in das Verzeichnis `<YOUR-SITE-COLLECTION-URL>/SitePages/CustomLearningAdmin.aspx`. Beim Öffnen von **CustomLearningAdmin. aspx** wird das **CustomConfig** -Listenelement initialisiert, das Lern Pfade für die erste Verwendung einrichtet. Sie sollten eine Seite sehen, die wie folgt aussieht:

![cg-adminapppage.png](media/cg-adminapppage.png)

## <a name="add-owners-to-site"></a>Hinzufügen von Besitzern zur Website
Als mandantenadministrator ist es unwahrscheinlich, dass Sie die Person anpassen, die die Website anpasst, sodass Sie der Website einige Besitzer zuweisen müssen. Besitzer verfügen über Administratorrechte für die Website, damit Sie Website Seiten ändern und die Website neu Branding können. Außerdem können Sie Inhalte, die über das Lern Pfade-Webpart übermittelt werden, ausblenden und anzeigen. Darüber hinaus haben Sie die Möglichkeit, benutzerdefinierte Wiedergabelisten zu erstellen und Sie benutzerdefinierten Unterkategorien zuzuweisen.  

1. Klicken Sie im Menü SharePoint- **Einstellungen** auf **Websiteberechtigungen**.
2. Klicken Sie auf **Erweiterte Berechtigungseinstellungen**.
3. Klicken Sie auf **Lern Pfade für Office 365 Besitzer**.
4. Klicken Sie auf **neu**  >  **Hinzufügen von Benutzern zu dieser Gruppe**, und fügen Sie dann die Personen hinzu, die Besitzer sein sollen. 
5. Fügen Sie einen Link zum [Durchsuchen der Website](https://docs.microsoft.com/Office365/CustomLearning/custom_explore) in der Freigabenachricht hinzu, und klicken Sie dann auf **Freigeben**.

## <a name="migrate-custom-content"></a>Migrieren von benutzerdefinierten Inhalten
Nachdem Sie die Website für Lernpfade wiederhergestellt haben, indem Sie die obigen Schritte ausführen, müssen Sie den Inhalt Ihrer **CustomPlaylists** -Liste und ihrer **CustomAssets** -Liste verlagern. Sie können auch die tatsächlichen benutzerdefinierten Seiten, aus denen sich Ihre benutzerdefinierten Objekte zusammensetzen, wahlweise in der vorhandenen Lern Pfad-Website verlagern, und ihre Absicht besteht darin, diese zu löschen. Die Aufgabe kann schwierig sein, da für alle Elemente in der **CustomPlaylists** -Liste die ID des Listenelements in der **CustomAssets** -Liste im Feld JSONData jedes Listenelements für eine Wiedergabeliste begraben ist. Daher reicht das einfache Verschieben des Inhalts der **CustomPlaylists** -Liste von einer Website zur anderen nicht aus. Außerdem enthält die **CustomAssets** -Liste die absolute URL der benutzerdefinierten Ressourcen Seite im Feld JSONData des Listenelements. Wenn die Objekte nicht verschoben werden und die Website nicht umbenannt wird (wodurch die absolute URL auf die Seite der Ressource geändert wird), kann **CustomAssets** bleiben. Die Einträge müssen jedoch manuell korrigiert werden. In Anbetracht der Komplexität dieser Art von Migration empfehlen wir Ihnen, einen unserer Partner für Lern Pfade einzutragen, um Sie bei der Durchführung dieses Übergangs zu unterstützen. 

### <a name="next-steps"></a>Nächste Schritte
- Siehe [Anpassen von Lernpfaden](custom_overview.md). 
- Weitere Informationen finden Sie unter [Translate site Pages](custom_translate_page_ml.md).


