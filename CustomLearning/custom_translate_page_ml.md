---
author: pkrebs
ms.author: pkrebs
title: Übersetzen von Websiteseiten
ms.date: 07/06/2020
description: Übersetzen von Websiteseiten
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: baa46deda7d7e10f3a7655fc6da076d37607e29f
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000291"
---
# <a name="translate-site-pages"></a>Übersetzen von Websiteseiten
Bevor Sie mit der Übersetzung der Lernpfadwebsite beginnen, ist es wichtig, einige wichtige Konzepte zu verstehen, wie das mehrsprachige Feature mit Lernpfaden funktioniert. 
- Websiteinformationen – Navigations-, Logo- und Websitenamenübersetzungen erfordern, dass die Website im Sprachprofil des Benutzers angezeigt und übersetzt wird.  
- Das Web part für Lernpfade muss mit dem Sprachprofil des Benutzers angezeigt werden, damit es in einer nicht englischen Sprache angezeigt wird. Das Webteil und die von Microsoft bereitgestellten Inhalte sind bereits für Sie übersetzt. Weitere Informationen zu Sprachprofilen finden Sie [unter Change your personal language and regional settings](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7).
- Die Art und Weise, wie Sie Lernpfade einrichten, bestimmt, ob Sie über übersetzte Seiten verfügen. Neue Websites, die mit dem Microsoft 365-Look-Book-Dienst bereitgestellt werden, verfügen über übersetzte Seiten in neun Sprachen. Aktualisierte Websites oder Websites, die Sie erstellen, erfordern eine manuelle Übersetzung. Weitere [Informationen finden Sie unter Setupoptionen für mehrsprachige Lernpfade](custom_setupoptions_ml.md).
- Multilingual support for learning pathways is enabled by SharePoint Online multilingual features for communication sites. Weitere Informationen zu mehrsprachigen SharePoint Online-Features finden Sie unter [Create multilingual communication sites, pages, and news](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c). 

## <a name="working-with-a-newly-provisioned-site"></a>Arbeiten mit einer neu bereitgestellten Website
Wenn Sie eine neue Lernpfadwebsite aus dem Microsoft 365-Look-Book-Dienst bereitgestellt haben, stehen Ihnen die übersetzten Seiten bereits zur Verfügung. Standardmäßig stellt die Website die folgenden Seiten zur Verfügung:

- Home.aspx
- Start-with-Six-Simple-Steps.aspx
- Erste Schritte mit Microsoft-365.aspx
- Get-started-with-Microsoft-Teams.aspx
- Get-started-with-SharePoint.aspx
- Get-started-with-OneDriive.aspx
- Ask-questions-and-get-help.aspx
- Schulungsereignisse calendar.aspx
- Become-a-Champion.aspx
- Recommended-Playlists.aspx
- Lernpfade Admin Success Center

## <a name="view-translated-pages-from-the-newly-provisioned-site"></a>Anzeigen übersetzter Seiten von der neu bereitgestellten Website
Um sich mit der Website für übersetzte Lernpfade vertraut zu machen, werfen wir einen Blick auf einige übersetzte Seiten.

### <a name="view-the-translated-home-page"></a>Anzeigen der übersetzten Homepage
Wählen Sie auf der Startseite der Lernpfade eine Sprache aus dem Sprachdropdown aus, wie im folgenden Beispiel gezeigt. Im Beispiel wird Italienisch in der oberen rechten Ecke ausgewählt angezeigt, und alle Seitenelemente werden übersetzt.

![Fotos der verwendeten Lernpfade](media/custom_ml_pages_home.png)

### <a name="view-the-translated-microsoft-365-training-page"></a>Anzeigen der übersetzten Microsoft 365-Schulungsseite
Sehen wir uns nun die Microsoft 365-Schulungsseite an. 

1. Klicken Sie auf der Startseite **der** Lernpfadwebsite auf **Microsoft 365-Schulungen.**
2. Wählen Sie in der oberen rechten Ecke der Seite eine Sprache aus. In diesem Beispiel wird Italienisch ausgewählt.

![Beispielseite für Lernpfade für Italienisch.](media/custom_ml_pages_training.png)

Welche Übersetzungen werden angezeigt, wenn die Sprache ausgewählt ist?
- Die SharePoint-Seite wird wie in der obigen Grafik dargestellt übersetzt. Beachten Sie, dass der Text für das Seitenbanner jetzt auf Italienisch angezeigt wird.

Welche Übersetzungen sind nicht sichtbar?
- Der Websitename ist in Englisch
- Die Websitenavigation ist in Englisch
- Das Web part für Lernpfade ist in Englisch

## <a name="view-the-fully-translated-site"></a>Anzeigen der vollständig übersetzten Website 
Zum Anzeigen einer vollständig übersetzten Website in einer bestimmten Sprache, einschließlich Websiteseiten, Navigation und Webteil, müssen die persönliche Sprache und die regionalen Einstellungen des Benutzers für diese Sprache festgelegt werden. Weitere Informationen zum Festlegen von Sprach- und Regionaleinstellungen finden Sie [unter Change your personal language and regional settings](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7). Es wird empfohlen, dass Sie ein separates Konto verwenden oder einen anderen Benutzer mit den verschiedenen Spracheinstellungen die übersetzten Seiten anzeigen.  

## <a name="working-with-an-updated-or-manually-installed-learning-pathways-site"></a>Arbeiten mit einer aktualisierten oder manuell installierten Lernpfadwebsite
Wenn Sie eine vorhandene Lernpfadwebsite aktualisiert oder das Webteil manuell auf einer vorhandenen Website installiert haben, müssen Sie die Websiteseiten manuell übersetzen. Das Webteil und die Inhalte der Lernpfade sind bereits übersetzt und werden in der bevorzugten Sprache des Benutzers angezeigt. Informationen zum Übersetzen von Seiten finden Sie in den folgenden Anweisungen "Erstellen von Seiten für die sprachen, die Sie möchten". 

## <a name="create-pages-for-the-languages-you-want"></a>Erstellen von Seiten für die sprachen, die Sie möchten
Nachdem Sie Ihre Website für mehrsprachige Features aktiviert haben und die sprachen ausgewählt haben, die Sie verfügbar machen möchten, können Sie die gewünschten Übersetzungsseiten erstellen. 

1. Wechseln Sie zur Standardsprachenseite, die Sie in einer anderen Sprache verfügbar machen möchten.
2. Wählen Sie auf der oberen Leiste **Übersetzung aus.**
3. Wählen **Sie Erstellen** für die sprachen aus, die Sie möchten.

> [!IMPORTANT]
> Nachdem Sie die Übersetzungsseiten erstellt haben, müssen Sie die Standardsprachenseite veröffentlichen (oder erneut veröffentlichen), um sicherzustellen, dass:
>- Übersetzungsseiten werden auf der entsprechenden Sprachwebsite angezeigt.
>- Übersetzungsseiten werden im News-Webparts und in den Webparts für hervorgehobene Inhalte ordnungsgemäß angezeigt.
>- Das Sprachdropdown oben auf der Website enthält alle sprachen, die Sie aktiviert haben.
>- Übersetzer werden über die Übersetzungsanforderung benachrichtigt.

Nachdem Sie die Seiten erstellt haben, wird der Status der Seite (Entwurf gespeichert, veröffentlicht und so weiter) im Übersetzungsbereich neben jeder Sprache angezeigt. Außerdem werden die von Ihnen zugewiesenen Übersetzer per E-Mail benachrichtigt, dass eine Übersetzung angefordert wird.

### <a name="view-the-fully-translated-site-in-a-specific-language"></a>Anzeigen der vollständig übersetzten Website in einer bestimmten Sprache
Zum Anzeigen einer vollständig übersetzten Website in einer bestimmten Sprache, einschließlich Websiteseiten, Navigation und Webteil, müssen die persönliche Sprache und die regionalen Einstellungen des Benutzers für diese Sprache festgelegt werden. Weitere Informationen zum Festlegen von Sprach- und Regionaleinstellungen finden Sie [unter Change your personal language and regional settings](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7). Beachten Sie, dass es am besten ist, ein separates Konto zu verwenden oder einen anderen Benutzer mit den verschiedenen Spracheinstellungen die übersetzten Seiten anzeigen zu können.

## <a name="what-does-a-translator-do"></a>Was macht ein Übersetzungstool?
 Nachdem die Website auf Englisch eingerichtet wurde, bearbeitet ein Benutzer mit Spanisch als bevorzugte persönliche Sprache z. B. den Titel, die Navigation und die Fußzeile manuell und übersetzt sie in Spanisch. Ein Benutzer mit Deutsch als bevorzugter persönlicher Sprache macht das gleiche für Deutsch. Nach der Übersetzung des Inhalts wird er für alle Benutzer dieser bevorzugten Sprachen angezeigt. Das Webteil nimmt die bevorzugte Sprache des Benutzers auf und zeigt die in dieser Sprache übersetzten Inhalte an. 

Übersetzer übersetzen die Kopien der Standardsprachenseite manuell in die angegebene Sprache. Wenn die Kopien der Seiten erstellt werden, werden die Übersetzer per E-Mail benachrichtigt, wenn ein Übersetzer angegeben wurde. Die E-Mail enthält einen Link zur Standardsprachenseite und zur neu erstellten Übersetzungsseite. Der Übersetzer hat:
1. Wählen Sie die **Schaltfläche Übersetzen** starten in der E-Mail aus.
2. Wählen **Sie oben** rechts auf der Seite Bearbeiten aus, und übersetzen Sie den Inhalt.
3. Wenn sie fertig sind, wählen Sie Als Entwurf speichern **aus** (wenn Sie nicht bereit sind, ihn für Leser sichtbar zu machen) oder wenn die Seite für alle Benutzer dieser Sprache auf der Website sichtbar sein kann, wählen Sie **Veröffentlichen** oder Veröffentlichen von Nachrichten **aus.**

Weitere Informationen zum Übersetzungsprozess finden Sie unter [Create multilingual communication sites, pages, and news](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c). 

## <a name="updating-the-default-language-page"></a>Aktualisieren der Standardsprachenseite
Wenn die Standardsprachenseite aktualisiert wird, muss die Seite erneut veröffentlicht werden. Anschließend werden die Übersetzer für die Übersetzungsseiten per E-Mail benachrichtigt, dass ein Update vorgenommen wurde, damit Aktualisierungen an den einzelnen Übersetzungsseiten vorgenommen werden können.

## <a name="set-up-a-multilingual-site-name-navigation-and-footer"></a>Einrichten eines mehrsprachigen Websitenamens, einer Navigation und einer Fußzeile
Wenn Sie den Websitenamen, die Navigation und die Fußzeile Ihrer Website in den verschiedenen Sprachen, die Sie zur Verfügung gestellt haben, anzeigen möchten, müssen Sie diese manuell übersetzen.

Nehmen wir beispielsweise an, Sie haben eine Kommunikationswebsite mit einer englischen Standardsprache erstellt und Sie haben die Website für Spanisch und Deutsch aktiviert. Wenn Sie eine Website erstellen, richten Sie den Websitenamen und die Beschreibung in der Standardsprache (in diesem Fall Englisch) ein. Sie können den Websitenamen und die Beschreibung auch nach der Websiteerstellung aktualisieren. Anschließend erstellen Sie die Navigationsknoten und den Fußzeileninhalt auf Englisch.

Nachdem die Website auf Englisch eingerichtet wurde, werden die Inhalte für Titel, Beschreibung, Navigation und Fußzeile von einem Benutzer mit Spanisch als seine bevorzugte persönliche Sprache manuell bearbeitet und auf Spanisch übersetzt. Ein Benutzer mit Deutsch als bevorzugter persönlicher Sprache macht das gleiche für Deutsch. Nach der Übersetzung des Inhalts wird er für alle Benutzer dieser bevorzugten Sprachen angezeigt. 

> [! HINWEISE]
>- Benutzer, die die Websiteinhalte für ihre bevorzugten Sprachen übersetzen, sollten Mitglieder der Gruppe Besitzer für die Website sein oder über entsprechende Websiteberechtigungen verfügen.
>- Wenn eine Änderung am Websitenamen, der Navigation oder der Fußzeile in der Standardsprache vorgenommen wird, wird das entsprechende übersetzte Element in einer anderen Sprache nicht automatisch aktualisiert, es sei denn, Sie möchten vorhandene Websiteübersetzungen überschreiben. Wenn Sie dies tun, wird das übersetzte Element durch das Update in der Standardsprache ersetzt und müsste erneut manuell übersetzt werden. Um Übersetzungen zu überschreiben, wechseln Sie zur Seite Websitesprachen für die Standardsprache, und wählen Sie Erweiterte Einstellungen anzeigen aus. Verschieben Sie dann die Umschalte für Übersetzungen überschreiben in On. Diese Option gilt nicht für Seiten- oder Nachrichteninhalte.

### <a name="to-view-the-fully-translated-site-in-a-specific-language"></a>So zeigen Sie die vollständig übersetzte Website in einer bestimmten Sprache an
Zum Anzeigen einer vollständig übersetzten Website in einer bestimmten Sprache, einschließlich Websiteseiten, Navigation und Webteil, müssen die persönliche Sprache und die regionalen Einstellungen des Benutzers für diese Sprache festgelegt werden. Weitere Informationen zum Festlegen von Sprach- und Regionaleinstellungen finden Sie [unter Change your personal language and regional settings](https://support.microsoft.com/office/change-your-personal-language-and-region-settings-caa1fccc-bcdb-42f3-9e5b-45957647ffd7). Es wird empfohlen, dass Sie ein separates Konto verwenden oder einen anderen Benutzer mit den verschiedenen Spracheinstellungen die übersetzten Seiten anzeigen.

## <a name="for-more-information"></a>Weitere Informationen
- Weitere Informationen zum Übersetzen von SharePoint-Kommunikationswebsiteseiten finden Sie unter [Create multilingual communication sites, pages, and news](https://support.office.com/article/2bb7d610-5453-41c6-a0e8-6f40b3ed750c).
- Weitere Informationen zum Anpassen von Lernpfaden finden Sie unter [Customize Learning Pathways](custom_overview.md).  
