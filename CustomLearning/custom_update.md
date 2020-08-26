---
author: pkrebs
ms.author: pkrebs
title: Aktualisieren von Microsoft 365 Lernpfaden
ms.date: 07/06/2020
description: Aktualisieren von Microsoft 365 Lernpfaden
ms.openlocfilehash: 6880e49f925f18b961790ec9eff2fbca55a741b7
ms.sourcegitcommit: a34d166d01e0a0a0f7d36593ad69b93e923d778b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/26/2020
ms.locfileid: "46895583"
---
# <a name="update-learning-pathways"></a>Lernpfade aktualisieren
Wenn Sie über eine vorhandene Lern Pfad Website verfügen, können Sie diese für mehrsprachige Unterstützung aktualisieren. Um Lern Pfade auf die mehrsprachige Version 4,0 zu aktualisieren, laden Sie das Webpart-Paket, customlearning. sppkg, in den SharePoint-Mandanten-App-Katalog hoch. Beim Aktualisieren von Lernpfaden:  

- Zuvor erstellte benutzerdefinierte Wiedergabelisten und Objekte werden beibehalten.
- Einstellungen zum Ausblenden oder Anzeigen von Inhalten werden beibehalten
- Die SharePoint-Vorlage für Lern Pfade bleibt unverändert
- Die Website Seiten für Lern Pfade werden nicht übersetzt. Diese Arbeit muss manuell durchgeführt werden.

## <a name="read-the-learning-pathways-multilingual-overview"></a>Lesen der Lern Pfade – mehrsprachig (Übersicht)
Weitere Informationen zur Funktionsweise der mehrsprachigen Unterstützung für Lern Pfade finden Sie in den [Lernpfaden mehrsprachig (Übersicht](custom_overview.md)). 

## <a name="prerequisites-to-update"></a>Voraussetzungen für die Aktualisierung
Vor dem Aktualisieren von Lernpfaden müssen folgende Voraussetzungen erfüllt sein:
- Die Person, die Lern Pfade aktualisiert, muss ein Websitesammlungsbesitzer des Mandanten-App-Katalogs sein. Wenn die Person, die Lernpfade ausstellt, kein Websitesammlungsbesitzer des App-Katalogs ist, führen Sie die [folgenden Schritte](addappadmin.md) aus, und fahren Sie fort. 

## <a name="set-language-settings"></a>Festlegen von Spracheinstellungen 
Legen Sie vor dem Aktualisieren von Lernpfaden die Einstellungen für die Website Sprache fest. Um die mehrsprachige Unterstützung für die Website für Lern Pfade zu aktivieren, können Sie die **Option Seiten und Nachrichten aktivieren in mehrere Sprachen** auf **ein**setzen festlegen und dann die Sprachen hinzufügen, die Sie für die Website unterstützen möchten.
1.  Wählen Sie auf der Website Lern Pfade die Option **Einstellungen** von oben rechts aus, und wählen Sie dann **Website Informationen**aus.
2.  Wählen Sie unten im Bereich Website Informationen die Option **Alle Websiteeinstellungen anzeigen**aus.
3.  Wählen Sie unter **Websiteverwaltung**die Option **Spracheinstellungen**aus.
4.  Legen **Sie unter Aktivieren von Seiten und Nachrichten in mehrere Sprachen übersetzt**den Umschaltfläche-Schalter fest. 
- Für eine mehrsprachigen-Website schieben Sie die Umschaltfläche **auf**ein, und fahren Sie dann mit dem Abschnitt Sprachen hinzufügen fort. 
- Bei einer nur-Englisch-Website schieben Sie die Umschaltfläche auf **aus**.

### <a name="add-languages"></a>Hinzufügen von Sprachen
Lern Pfade unterstützen neun Sprachen, Sie sollten nur die Sprachen hinzufügen, die Sie benötigen. In den in dieser Dokumentation verwendeten Beispielen wird Italienisch hinzugefügt. 
- Geben Sie unter **Sprachen hinzufügen oder entfernen**die Eingabe eines sprach namens in **"auswählen" oder**"Sprache eingeben" ein, oder wählen Sie eine Sprache aus der Dropdownliste aus. Sie können diesen Schritt wiederholen, um mehrere Sprachen hinzuzufügen. Sie können jederzeit Sprachen von Ihrer Website hinzufügen oder entfernen, indem Sie zurück zu dieser Seite wechseln.
 
### <a name="assign-translators"></a>Zuweisen von Übersetzern
Beim Definieren von Spracheinstellungen für Lern Pfade können Sie Übersetzer zuweisen. Für Übersetzer sollte ein Fremdsprachen Profil eingerichtet sein. Weitere Informationen zu fremdsprachigen Profilen finden Sie unter [Erstellen von mehrsprachigen Kommunikationswebsites, Seiten und Nachrichten](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).  
- Klicken Sie für eine unterstützte Sprache auf **auswählen, oder geben Sie einen Übersetzer** ein, und wählen Sie dann einen Übersetzer aus. 

## <a name="update-the-learning-pathways-web-part-package"></a>Aktualisieren des Lern Pfad-Webparts-Pakets
In diesem Schritt laden Sie das Lern Pfade 4,0-Webpart in den SharePoint-App-Katalog hoch, und navigieren Sie dann zur Seite Verwaltungstools für Lern Pfade, um den Updateprozess zu starten.

### <a name="upload-the-web-part-package"></a>Hochladen des Webpart-Pakets
1.  Wechseln Sie zum [benutzerdefinierten GitHub-Lern-Repository](https://github.com/pnp/custom-learning-office-365/tree/master/webpart), wählen Sie **customlearning. sppkg** aus, und laden Sie es dann auf ein lokales Laufwerk auf Ihrem PC herunter.
2.  Wenn Sie noch nicht angemeldet sind, melden Sie sich bei Ihrem Mandanten mit einem mandantenadministrator oder einem Websitesammlungsadministrator Konto an. 
3.  Klicken Sie auf **Admin**  >  **alle**  >  **SharePoint**  >  -**Funktionen**anzeigen. 
4.  Klicken Sie unter **apps**auf **Öffnen**. 
5.  Klicken Sie auf **App-Katalog**  >  **Apps für SharePoint verteilen**. 
6.  Klicken Sie auf **hochladen**  >  **Auswählen von Dateien**. 
7.  Wählen Sie die Datei **customlearning. sppkg** aus, die Sie heruntergeladen haben, und klicken Sie auf **OK**  >  **Deploy**. 

### <a name="complete-the-update"></a>Abschließen des Updates
1.  Wählen Sie auf der Website Lernpfade im Menü **Start** die Option **Verwaltung von Lernpfaden** aus. 
2.  Eine Eingabeaufforderung wird angezeigt, in der Sie gefragt werden, ob Sie aktualisieren möchten. 
![custom_update_adminprompt_ml.png](media/custom_update_adminprompt_ml.png)
3.  Klicken Sie auf **Start**. 
4. Wenn das Update abgeschlossen ist, klicken Sie auf **Schließen**. 

### <a name="next-steps"></a>Nächste Schritte
- Erkunden Sie die in der Website und im Webpart bereitgestellten [Standardinhalte](custom_exploresite.md) .
- Weitere Informationen zum Übersetzen von Website Seiten finden Sie unter [Translate site Pages](custom_translate_page_ml.md). 

