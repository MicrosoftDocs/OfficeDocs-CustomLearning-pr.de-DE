---
author: karuanag
ms.author: karuanag
title: Häufig gestellte Fragen zur benutzerdefinierten Schulung für Office 365-Lösungen
ms.date: 02/10/2019
description: Informationen zu häufig gestellten Fragen zur benutzerdefinierten Schulung für Office 365
ms.openlocfilehash: 7da1f3da197fc298c83eac89e3455312cba7a851
ms.sourcegitcommit: c60ca83b784f36b6f41b56ac193f7d58c750984e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/12/2019
ms.locfileid: "30543765"
---
# <a name="frequently-asked-questions"></a>Häufig gestellte Fragen

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a>1. Was sind die Anforderungen für die Installation von benutzerdefiniertem Learning für Office 365 in meine Mandanten Umgebung?

- SharePoint Online-und Kommunikationswebsites aktiviert.
- Die Person, die CLO365 bereitstellen soll, muss der mandantenadministrator des Zielmandanten für die Installation sein.
- Ein Mandanten-App-Katalog muss innerhalb der Option "Apps" im SharePoint Admin Center verfügbar sein.
- Die Person, die CLO365 bereitstellen soll, muss ein Websitesammlungsadministrator des App-Katalogs im Zielmandanten für die Installation sein.

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a>2. in welchen Sprachen ist benutzerdefiniertes lernen für Office 365 in verfügbar?

Benutzerdefiniertes lernen für Office 365 ist derzeit nur in englischer Sprache verfügbar. Die automatische End-to-End-propositionierung funktioniert nur mit englischen Mandanten. In zukünftigen Versionen können zusätzliche Sprachen hinzugefügt werden.

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>3. wie lange dauert es, bis die Website in unserer Mandanten Umgebung installiert wird?

Basierend auf unseren Tests der Installation sollte es weniger als 15 Minuten dauern. Dies umfasst nicht die Zeit, die zum Anpassen der Website an Ihre Anforderungen erforderlich ist.

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a>4. können wir das benutzerdefinierte Learning für Office 365 zu einer Unterwebsite unserer primären SharePoint-Websitesammlung machen?

Nein. Die Website basiert auf einer Kommunikationswebsite Vorlage, die immer als Stammwebsitesammlung gedacht ist.

> [!NOTE]
> Es ist wichtig, die Berechtigungen zu berücksichtigen, die Ihre Endbenutzer für den Zugriff auf die Website benötigen. Die meisten Organisationen haben Sicherheits-oder Benutzergruppen definiert. Sie müssen dem neuen Schulungsportal die entsprechenden Sicherheitsgruppen hinzufügen, sobald Sie bereit sind, es in Ihrer Mitarbeiter Community zu starten.

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a>5. ich muss die Website neu installieren; Was soll ich tun?

BeFolgen Sie die [hier](custom_provision.md)veröffentlichten Installationsanweisungen.

> [!NOTE]
> Wenn Sie in Ihrer vorherigen Installation die Telemetrie deaktiviert hatten und die Telemetrie deaktiviert bleiben möchten, müssen Sie die Anweisungen zum Deaktivieren der Telemetrie hier befolgen.

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>6. Wir haben Updates für unsere Implementierung von Custom Learning für Office 365. Werden diese Updates (an Websitevorlage, Wiedergabelisten) verloren gehen, wenn wir die Website neu installieren?

Anpassungen an einzelnen Seiten und benutzerdefinierten Wiedergabelisten gehen verloren, wenn Sie die Website über Ihre aktuelle Installation neu installieren.  