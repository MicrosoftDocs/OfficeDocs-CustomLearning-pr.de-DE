---
author: pkrebs
ms.author: pkrebs
title: Setupoptionen für mehrsprachige Lernpfade
ms.date: 07/6/2020
description: Setupoptionen für mehrsprachige Lernpfade
ROBOTS: NOINDEX, NOFOLLOW
ms.service: sharepoint-online
manager: bpardi
ms.topic: article
audience: admin
ms.openlocfilehash: 1384885adc1d7119658bf968e18e8859c784ef37
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999311"
---
# <a name="setup-options-for-multilingual-learning-pathways"></a>Setupoptionen für mehrsprachige Lernpfade
Mit der Veröffentlichung mehrsprachiger Features für SharePoint Online-Kommunikationswebsites bieten Lernpfade jetzt Unterstützung für mehrere Sprachen. Sie können Lernpfade auf verschiedene Arten einrichten, um den Bedürfnissen Ihrer Organisation gerecht zu werden. Um Ihnen bei der Entscheidung über den besten Pfad für Ihre Organisation zu helfen, haben wir die Einstellungsoptionen behandelt. 

## <a name="new-install-scenarios"></a>Neue Installationsszenarien
In den "neuen Installationsszenarien" werden die Optionen zum Installieren einer neuen Instanz der Lernpfade mithilfe des SharePoint-Bereitstellungsdiensts erläutert, der jetzt im SharePoint-Look book verfügbar ist.

### <a name="scenario-1-we-have-not-installed-learning-pathways-and-need-learning-pathways-multilingual-support"></a>Szenario 1: Wir haben keine Lernpfade installiert und brauchen mehrsprachige Unterstützung für Lernpfade 
Wenn Sie keine Lernpfade installiert haben und mehrere Sprachen benötigen, können Sie den SharePoint-Bereitstellungsdienst verwenden, um eine neue Lösung für Lernpfade mit Unterstützung für neun Sprachen zu installieren. Englisch ist die Standardsprache und kann nicht geändert werden. 
- Informationen zur Bereitstellung einer neuen Lernpfade-Lösung mit Englisch als Standardsprache für die Website finden Sie unter [Bereitstellung einer neuen Lernpfade-Lösung](custom_provision_ml.md).

### <a name="scenario-2-we-installed-learning-pathways-but-arent-currently-using-it-andor-havent-made-any-customization-to-the-site-or-playlists"></a>Szenario 2: Wir haben Lernpfade installiert, verwenden sie aber derzeit nicht und/oder haben keine Anpassung an Website oder Wiedergabelisten vorgenommen. 
Wenn Sie Lernpfade installiert, aber nicht aktiv verwenden oder keine Anpassungen an der Website oder wiedergabelisten vorgenommen haben, können Sie den SharePoint-Bereitstellungsdienst verwenden, um eine neue Lösung mit Unterstützung für neun Sprachen zu installieren. Englisch ist die Standardsprache und kann nicht geändert werden. 
- Informationen zur Bereitstellung einer neuen Lernpfade-Lösung mit Englisch als Standardsprache für die Website finden Sie unter [Bereitstellung einer neuen Lernpfade-Lösung](custom_provision_ml.md).

### <a name="scenario-3-we-havent-installed-learning-pathways-and-dont-need-multilingual-support"></a>Szenario 3: Wir haben keine Lernpfade installiert und brauchen keinen mehrsprachigen Support 
Wenn Sie keine Lernpfade installiert haben und keinen mehrsprachigen Support benötigen, können Sie sie über den SharePoint-Bereitstellungsdienst installieren. Englisch ist die Standardsprache. Nach der Installation müssen Sie die Mehrsprachigkeit deaktivieren. 
- Informationen zur Bereitstellung einer neuen Lernpfade-Lösung ohne mehrsprachigen Support finden Sie unter [Bereitstellung einer neuen Lernpfade-Lösung](custom_provision_ml.md).

## <a name="update-learning-pathways-with-a-web-part-upload-scenarios"></a>Szenarien für das Aktualisieren von Lernpfaden (mit einem Webpartupload)
Wenn Sie eine vorhandene Version von Lernpfaden installiert haben, können Sie das Lernpfade-Webpart in den SharePoint-App-Katalog hochladen, um den mehrsprachigen Support zu aktivieren. 

### <a name="scenario-1-we-need-to-upgrade-an-existing-version-of-learning-pathways-but-dont-need-multilingual-support"></a>Szenario 1: Wir müssen eine vorhandene Version von Lernpfaden aktualisieren, benötigen aber keinen mehrsprachigen Support.
Sie können Version 4.0 der Lernpfade ohne mehrsprachigen Support aktualisieren. Mit dem Update erhalten Sie einige neue Features, einschließlich einer Bildauswahl für benutzerdefinierte Wiedergabelisten und Unterkategorien. 

- Wenn Sie eine vorhandene Lernpfade-Lösung ohne mehrsprachigen Support aktualisieren möchten, lesen Sie [Aktualisieren von Lernpfaden für mehrsprachigen Support](custom_update_ml.md). Der Upgradeprozess für Versionen ohne mehrsprachigen Support gleicht dem für mit Versionen mit mehrsprachigem Support, umfasst aber weniger Schritten. 

### <a name="scenario-2-we-need-to-upgrade-to-multilingual-support-and-the-default-language-of-the-site-collection-is-our-default-language"></a>Szenario 2: Wir müssen ein Upgrade auf eine Version mit mehrsprachigem Support durchführen, und die Standardsprache der Websitesammlung ist unsere Standardsprache.
Version 4.0 der Lernpfade unterstützt mehrsprachige Seiten in Ihrer Websitesammlung. Zusätzlich zu mehrsprachigem Support erhalten Sie einige neue Features, einschließlich einer Bildauswahl für benutzerdefinierte Wiedergabelisten und Unterkategorien. 
- Wenn Sie eine vorhandene Lernpfade-Website mit mehrsprachigem Support aktualisieren möchten, lesen Sie [Aktualisieren von Lernpfaden für mehrsprachigen Support](custom_update_ml.md). 

## <a name="update-learning-pathways-for-multilingual-support-with-manual-install"></a>Aktualisieren von Lernpfaden für mehrsprachigen Support mit der manuellen Installation 
Im Folgenden werden die Szenarien für die Aktualisierung einer bestehenden Instanz der Lernpfade-Lösung auf die mehrsprachige Version 4.0 durch manuelle Installation des Lernpfade-Webparts beschrieben. 

### <a name="scenario-1-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--no-custom-content"></a>Szenario 1: Wir benötigen mehrsprachigen Support, und die Standardsprache der Websitesammlung ist nicht unsere Standardsprache (kein benutzerdefinierter Inhalt). 
Version 4.0 der Lernpfade unterstützt dieses Szenario. In diesem Szenario wird jedoch angenommen, dass keine benutzerdefinierten Inhalte oder Wiedergabelisten auf der bestehenden Website vorhanden sind. In diesem Szenario können Sie eine neue SharePoint Online-Kommunikationswebsite mit Ihrer Standardsprache erstellen, das Webpart hochladen und dann Lernpfade mithilfe eines PowerShell-Skripts manuell einrichten. 
- Informationen zum Einrichten von Lernpfaden für mehrsprachigen Support in Ihrer Standardsprache finden Sie unter [Manuelle Installation von Lernpfaden für mehrsprachigen Support](custom_manualsetup_ml.md).

### <a name="scenario-2-we-need-multilingual-support-and-the-default-language-of-the-site-collection-is-not-our-default-language--plus-we-have-custom-content"></a>Szenario 2: Wir benötigen mehrsprachigen Support, und die Standardsprache der Websitesammlung ist nicht unsere Standardsprache (es ist benutzerdefinierter Inhalt vorhanden). 
In diesem Szenario können Sie eine neue SharePoint Online-Kommunikationswebsite mit Ihrer Standardsprache erstellen, das Webpart hochladen und dann Lernpfade mithilfe eines PowerShell-Skripts manuell einrichten. 

Nachdem Sie Ihre Lernpfade-Website anhand der oben beschriebenen Schritte wieder eingerichtet haben, müssen Sie den Inhalt Ihrer Listen **CustomPlaylists** und **CustomAssets** verschieben. Sie können optional auch die tatsächlichen benutzerdefinierten Seiten, aus denen sich Ihre benutzerdefinierten Objekte zusammensetzen, verschieben, wenn sie in der bestehenden Lernpfade-Website vorhanden sind und Sie beabsichtigen, sie zu löschen. Die Aufgabe kann schwierig sein, da für alle Elemente in der Liste **CustomPlaylists** die ID des Listenelements in der Liste **CustomAssets** im Feld "JSONData" des jeweiligen Wiedergabelistenelements verborgen ist. Daher reicht es nicht aus, einfach den Inhalt der Liste **CustomPlaylists** von einer Website auf eine andere zu verschieben. Außerdem enthält die Liste **CustomAssets** die absolute URL für die Seite des benutzerdefinierten Objekts im Feld "JSONData" des Listenelements. Wenn die Objekte nicht verschoben werden und die Website nicht umbenannt (also die absolute URL der Seite des Objekts geändert) wird, kann **CustomAssets** beibehalten werden. Sie müssen die Einträge aber manuell korrigieren. Angesichts der Komplexität dieser Art von Migration sollten Sie erwägen, einen unserer Lernpfade-Partner in Anspruch zu nehmen, um Ihnen bei der Durchführung dieses Übergangs zu helfen.
- Informationen zum Einrichten von Lernpfaden für mehrsprachigen Support in Ihrer Standardsprache finden Sie unter [Manuelle Installation von Lernpfaden für mehrsprachigen Support](custom_manualsetup_ml.md).

