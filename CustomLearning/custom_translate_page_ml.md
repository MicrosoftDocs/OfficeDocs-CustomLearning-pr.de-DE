---
author: pkrebs
ms.author: pkrebs
title: Übersetzen von Website Seiten
ms.date: 02/10/2019
description: Übersetzen von Website Seiten
ms.openlocfilehash: 32dc0928d12074575c8608cef38e4b4d0e5e5cf3
ms.sourcegitcommit: 46caa9fa9d129bee107a8c9a7c5bc70a7f9af087
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/11/2020
ms.locfileid: "44699066"
---
# <a name="translate-site-pages"></a>Übersetzen von Website Seiten
Unabhängig davon, ob Sie eine vorhandene Version von Lernpfaden auf Version 4,0 aktualisiert haben oder eine neue Website bereitgestellt haben, ist das Verfahren zum Übersetzen von Website Seiten identisch. Es gibt jedoch einige Dinge, die Sie beachten sollten. 
- Wenn eine neue Lern Pfade mehrsprachig 4,0 Version vorgesehen ist, werden die Website Seiten für Sie in 9 Sprachen übersetzt. 
- Wenn die Lern Pfad Lösung auf die mehrsprachige Version von 4,0 aktualisiert wird, bleiben die Seiten der SharePoint-Website für Lern Pfade unverändert. Übersetzungen müssen manuell erfolgen. 

Die Website für Lern Pfade stellt standardmäßig die folgenden Seiten bereit:

- Home. aspx
- Start-with-Six-Simple-Steps. aspx
- Get-Started-with-Microsoft-365. aspx
- Get-Started-with-Microsoft-Teams. aspx
- Get-Started-with-SharePoint. aspx
- Get-Started-with-OneDriive. aspx
- Ask-questions-and-Get-Help. aspx
- Schulungs Ereignisse Calendar. aspx
- Become-a-Champion. aspx
- Recommended-Playlists. aspx
- Lern Pfade Administrator Success Center

## <a name="create-pages-for-the-languages-you-want"></a>Erstellen von Seiten für die gewünschten Sprachen
Nachdem Sie Ihre Website für mehrsprachige Funktionen aktiviert haben und die Sprachen ausgewählt haben, die Sie zur Verfügung stellen möchten, können Sie die gewünschten Übersetzungsseiten erstellen. Um einige wichtige Konzepte veranschaulichen zu können, verwenden wir die Microsoft 365-Schulungsseite als Beispiel. Gehen Sie hierfür folgendermaßen vor:

1.  Klicken Sie auf der **Start** Seite für Lern Pfade auf **Microsoft 365 Training**.  
2.  Wählen Sie in der oberen Leiste **Übersetzung**aus.
![custom_update_ml_transbutton.png](media/custom_update_ml_transbutton.png)
3. Wenn Sie eine Seite für die Übersetzung in jeder für Ihre Website verfügbaren Sprache erstellen möchten, wählen Sie **für alle Sprachen erstellen**aus. Wählen Sie andernfalls nur für die gewünschten Sprachen **Erstellen** aus. In diesem Beispiel wählen Sie Italienisch aus.
4.  Klicken Sie auf **Ansicht**. Die Seite ist jetzt für die Übersetzung verfügbar. 

### <a name="an-important-concept-to-know"></a>Ein wichtiges Konzept, das Sie kennen sollten
Beachten Sie, dass im folgenden Beispiel die Seite in Italienisch übersetzt wurde. Der Website Titel, die Navigation und das Webpart werden jedoch weiterhin in Englisch angezeigt. 

![custom_update_ml_transpgconcept.png](media/custom_update_ml_transpgconcept.png)

 Nachdem die Website in Englisch eingerichtet wurde, wird ein Benutzer mit Spanisch, beispielsweise als bevorzugter persönlicher Sprache, die Titel-, Navigations-und Fußzeilen Inhalte manuell in Spanisch bearbeitet und übersetzt. Ein Benutzer mit Deutsch als bevorzugter persönlicher Sprache macht dasselbe für Deutsch. Sobald der Inhalt übersetzt wurde, wird er für alle Benutzer dieser bevorzugten Sprachen angezeigt. Das Webpart nimmt die bevorzugte Sprache des Benutzers auf und zeigt den Inhalt an, der in dieser Sprache übersetzt wurde. 

> [!IMPORTANT]
> Wichtig: Nachdem Sie die Übersetzungsseiten erstellt haben, müssen Sie die standardmäßige englischsprachige Seite veröffentlichen (oder erneut veröffentlichen), um Folgendes sicherzustellen:
- Übersetzungsseiten werden auf der entsprechenden sprach Website angezeigt.
- Übersetzungsseiten werden ordnungsgemäß im News-Webpart und den markierten Inhalts Webparts angezeigt
- Das Sprachmenü oben auf der Website enthält alle Sprachen, die Sie aktiviert haben.
- Übersetzer werden über die Übersetzungsanforderung benachrichtigt.

## <a name="what-does-a-translator-do"></a>Was macht ein Übersetzungstool?
Übersetzer übersetzen die Kopien der Standardsprach Seite manuell in die angegebenen Sprache (n). Wenn die Kopien der Seite (n) erstellt werden, werden Übersetzer per e-Mail benachrichtigt. Die e-Mail enthält einen Link zur Standardsprach Seite und der neu erstellten Übersetzungsseite. Der Übersetzer wird:
1. Wählen Sie die Schaltfläche über **Setzung starten** in der e-Mail aus.
2. Wählen Sie oben rechts auf der Seite **Bearbeiten** aus, und übersetzen Sie den Inhalt.
3. Wenn Sie fertig sind, wählen Sie **als Entwurf speichern** (wenn Sie nicht bereit sind, es für Leser sichtbar zu machen) oder, wenn die Seite für jeden sichtbar ist, der diese Sprache auf der Website verwendet, die Option **veröffentlichen oder veröffentlichen** von **Nachrichten**auswählen.

Weitere Informationen zum Übersetzungsprozess finden Sie unter [Erstellen von mehrsprachigen Kommunikationswebsites, Seiten und Nachrichten](https://support.office.com/en-us/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c). 

## <a name="updating-the-default-language-page"></a>Aktualisieren der Standardsprach Seite
Wenn die Seite Standardsprache aktualisiert wird, muss die Seite erneut veröffentlicht werden. Anschließend werden die Übersetzer für die Übersetzungsseiten per e-Mail benachrichtigt, dass eine Aktualisierung vorgenommen wurde, damit die einzelnen Übersetzungsseiten aktualisiert werden können.

## <a name="next-steps"></a>Nächste Schritte
- [Übersetzen benutzerdefinierter Wiedergabelisten](custom_translate_pl_ml.md)
- [Ausblenden und Anzeigen von mehrsprachigen-Inhalten](custom_translate_pl_ml.md)
