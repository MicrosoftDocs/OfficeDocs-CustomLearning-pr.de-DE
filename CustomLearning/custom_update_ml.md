---
author: pkrebs
ms.author: pkrebs
title: Aktualisieren von Lernpfaden für mehrsprachigen Support
ms.date: 05/20/2019
description: Aktualisieren von Lernpfaden für mehrsprachigen Support
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 9344cd91e5b6718b1eb0e73e25fdc8311afed793
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000241"
---
# <a name="update-learning-pathways-for-multilingual-support"></a>Aktualisieren von Lernpfaden für mehrsprachigen Support
Wenn Sie über eine vorhandene Website für Lernpfade verfügen, können Sie sie für mehrsprachigen Support aktualisieren. Um Lernpfade auf die mehrsprachige Version 4.0 zu aktualisieren, laden Sie das Webteilpaket customlearning.sppkg in den SharePoint-Mandanten-App-Katalog hoch. Wenn Sie Lernpfade aktualisieren:  

- Alle zuvor erstellten benutzerdefinierten Wiedergabelisten und Ressourcen werden verwaltet
- Einstellungen zum Ausblenden oder Anzeigen von Inhalten werden beibehalten
- Die SharePoint-Vorlage für Lernpfade bleibt unverändert
- Die Seiten der Lernpfade werden nicht übersetzt. Diese Arbeit muss manuell durchgeführt werden

## <a name="read-the-learning-pathways-multilingual-overview"></a>Mehrsprachige Übersicht über Lernpfade lesen
Informationen dazu, wie mehrsprachiger Support für Lernpfade funktioniert, finden Sie in der Mehrsprachigen Übersicht über [Lernpfade](custom_overview_ml.md)). 

## <a name="prerequisites-to-update"></a>Zu aktualisierende Voraussetzungen
Vor dem Aktualisieren von Lernpfaden muss die folgende Voraussetzung erfüllt sein:
- Die Person, die Lernpfade aktualisiert, muss Websitesammlungsbesitzer des Mandanten-App-Katalogs sein. Wenn die Person, die Lernpfade bereitstellen, kein Websitesammlungsbesitzer des App-Katalogs ist, führen Sie [diese](addappadmin.md) Anweisungen aus, und fahren Sie fort. 

## <a name="set-language-settings"></a>Festlegen von Spracheinstellungen 
Legen Sie vor dem Aktualisieren von Lernpfaden die Spracheinstellungen für die Website ein. Um die mehrsprachige Unterstützung für die Lernpfadwebsite  zu aktivieren, können Sie die Option Seiten und Nachrichten aktivieren, die in mehrere Sprachen übersetzt werden sollen, auf **Ein** festlegen und dann die Sprachen hinzufügen, die Sie für die Website unterstützen möchten.
1.  Wählen Sie auf der  Website Lernpfade oben rechts Einstellungen aus, und wählen Sie dann **Websiteinformationen aus.**
2.  Wählen Sie unten im Bereich Websiteinformationen die Option **Alle Websiteeinstellungen anzeigen aus.**
3.  Wählen **Sie unter Websiteverwaltung** die Option **Spracheinstellungen aus.**
4.  Legen **Sie unter Seiten und Nachrichten in mehrere** Sprachen übersetzen aktivieren den Umschalter ein. 
- Verschieben Sie für eine mehrsprachige Website den Umschalter auf **Ein**, und fahren Sie dann mit dem Abschnitt Sprachen hinzufügen fort. 
- Verschieben Sie für eine englischsprachige Website den Umschalter auf **Aus**.

### <a name="add-languages"></a>Hinzufügen von Sprachen
Lernpfade unterstützen neun Sprachen, Sie sollten nur die benötigten Sprachen hinzufügen. In den in dieser Dokumentation verwendeten Beispielen wird Italienisch hinzugefügt. 
- Geben Sie unter Hinzufügen **oder Entfernen** von Websitesprachen einen Sprachnamen in **Auswählen** oder Eingeben einer Sprache ein, oder wählen Sie eine Sprache aus dem Dropdown aus. Sie können diesen Schritt wiederholen, um mehrere Sprachen hinzuzufügen. Sie können Ihrer Website jederzeit Sprachen hinzufügen oder entfernen, indem Sie zu dieser Seite zurückwechseln.
 
### <a name="assign-translators"></a>Zuweisen von Übersetzern
Beim Definieren von Spracheinstellungen für Lernpfade können Sie Übersetzer zuweisen. Für Übersetzer sollte ein Fremdsprachenprofil eingerichtet sein. Weitere Informationen zu Fremdsprachenprofilen finden Sie unter [Create multilingual communication sites, pages, and news](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).  
- Klicken Sie für eine unterstützte Sprache auf **Übersetzer auswählen** oder eingeben, und wählen Sie dann einen Übersetzer aus. 

## <a name="update-the-learning-pathways-web-part-package"></a>Aktualisieren des Web part-Pakets für Lernpfade
In diesem Schritt laden Sie das Webteil Lernpfade 4.0 in den SharePoint-App-Katalog hoch und navigieren dann zur Seite Verwaltung von Lernpfaden, um den Aktualisierungsprozess zu starten.

### <a name="upload-the-web-part-package"></a>Hochladen des Web part-Pakets
1.  Wechseln Sie zum [benutzerdefinierten GitHub-Lernrepository,](https://github.com/pnp/custom-learning-office-365/tree/master/webpart)wählen Sie **customlearning.sppkg** aus, und laden Sie es dann auf ein lokales Laufwerk auf Ihrem PC herunter. 
2.  Wenn Sie noch nicht angemeldet sind, melden Sie sich mit einem Mandantenadministrator- oder Sitesammlung-Administratorkonto bei Ihrem Mandanten an. 
3.  Klicken **Sie auf Administrator**  >  **Alle**  >  **SharePoint weitere** Features  >  **anzeigen**. 
4.  Klicken **Sie unter Apps** auf **Öffnen**. 
5.  Klicken **Sie auf App-Katalog**  >  **Apps für SharePoint verteilen**. 
6.  Klicken **Sie auf Dateien**  >  **hochladen**. 
7.  Wählen Sie die **datei customlearning.sppkg** aus, die Sie heruntergeladen haben, klicken Sie **auf OK**  >  **Bereitstellen**. 

### <a name="complete-the-update"></a>Abschließen des Updates
1.  Wählen Sie auf der Website Lernpfade im Menü Start die Option **Verwaltung von** **Lernpfaden** aus. 
2.  Es wird eine Eingabeaufforderung angezeigt, in der Sie gefragt werden, ob Sie aktualisieren möchten. 
![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)
3.  Klicken Sie auf **Start**. 
4. Klicken Sie nach Abschluss des Updates auf **Schließen**. 

### <a name="next-steps"></a>Nächste Schritte
- Sehen Sie sich [die Standardinhalte](custom_exploresite.md) an, die auf der Website und im Web part bereitgestellt werden.
- Weitere Informationen zum Übersetzen von Websiteseiten finden Sie unter [Translate site pages](custom_translate_page_ml.md). 

