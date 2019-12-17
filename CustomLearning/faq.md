---
author: karuanag
ms.author: karuanag
title: Häufig gestellte Fragen zu Microsoft 365-Lernpfaden
ms.date: 02/10/2019
description: Informationen zu häufig gestellten Fragen für Microsoft 365-Lern Pfade
ms.openlocfilehash: 5b90971ef6e411b4bd8d0cece2d8211f6fd5db23
ms.sourcegitcommit: 86cfa176d50b324c964b1a8609270cc73a2468b3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068816"
---
# <a name="frequently-asked-questions"></a>Häufig gestellte Fragen

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>Ich habe vor kurzem einen Blogbeitrag gesehen, bei dem benutzerdefiniertes lernen für Office 365 in Microsoft 365-Lern Pfade umbenannt wird. Werden der Lösung im Rahmen der Umbenennung weitere Änderungen hinzugefügt? Sollte ich die Lösung in meiner Organisation aktualisieren?

Die Microsoft 365-Lern Pfad Version ist eine neuausrichtungs Maßnahme, die dem Ändern des Namens der Lösung für das Microsoft 365-Branding gewidmet ist. Wenn Sie benutzerdefinierte Lernprogramm für Office 365 derzeit erfolgreich in Ihrer Organisation ausgeführt haben, ist es nicht erforderlich, die Lösung zu diesem Zeitpunkt zu aktualisieren.  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>Was sind die Voraussetzungen für die Installation von Microsoft 365-Lernpfaden in meiner Mandanten Umgebung?

- SharePoint Online-und Kommunikationswebsites aktiviert.
- Die Person, die CLO365 bereitstellen soll, muss der mandantenadministrator des Zielmandanten für die Installation sein.
- Ein Mandanten-App-Katalog muss in der Option "Apps" im SharePoint Admin Center verfügbar sein.
- Wenn ein neuer App-Katalog erstellt wird, ist eine Wartezeit von 30 Minuten oder mehr erforderlich, damit der APP-Katalog vollständig eingerichtet werden kann. Wenn Sie versuchen, Microsoft 365-Lern Pfade direkt nach dem Erstellen des Mandanten-App-Katalogs zur Verfügung zu stellen, führt dies zu einem Fehler bei der Bereitstellungslösung für die Lern Pfade. 
- Die Einzelperson, die CLO365 bereitstellen wird, muss ein Websitesammlungsadministrator des App-Katalogs im Zielmandanten für die Installation sein.

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Warum fragt Microsoft bei der Installation von Microsoft 365-Lernpfaden nach Mandanten Berechtigungen 

- Der SharePoint Online Bereitstellungsdienst verwendet die Berechtigungen, um die Lern Pfade SharePoint-Website zu erstellen, die Seiten der Website zu erstellen und die Microsoft 365-Lern Pfad Anwendung in Ihrem Mandanten zu installieren. Das ist der einzige Grund dafür, dass wir die Berechtigungen anfordern. Ohne die angeforderten Berechtigungen kann der SharePoint-Bereitstellungsdienst nicht die Befehle ausführen, die die Websitevorlage und das Webpart für Lern Pfade automatisch installieren. 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>Was sind die Auswirkungen von Microsoft 365-Lernpfaden in einer Beta Vorschau? 

Microsoft 365 Lern Pfade befinden sich derzeit in der Beta Vorschau. Berücksichtigen Sie beim Auswerten, planen und Implementieren von Microsoft 365-Lernpfaden Folgendes:

- Wie bei jeder Beta-Lösung behält sich unser Service Management Team das Recht vor, Änderungen am Dienst und an seinen Komponenten vorzunehmen. Da wir Bugs und UX-Probleme aktiv beheben, müssen Sie wahrscheinlich das Webpart aktualisieren.
- Um das Webpart zu aktualisieren, müssen Sie es aus unserem GitHub-Repository herunterladen und in ihren Mandanten-App-Katalog hochladen. Weitere Informationen finden Sie im Abschnitt "Aktualisieren der Lösung" der [Readme](https://github.com/pnp/custom-learning-office-365/blob/master/README.md) -Datei zu Microsoft 365 Learning-Pfaden. 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>In welchen Sprachen sind Microsoft 365-Lern Pfade verfügbar?

Microsoft 365-Lern Pfade sind derzeit nur in englischer Sprache verfügbar. Die automatische End-to-End-proprovisionierung funktioniert nur mit englischen Mandanten. Wir planen die Einführung einer mehrsprachigen Unterstützung für diese neun Sprachen im ersten Quartal 2020. 

- Chinesisch (vereinfacht) 
- Niederländisch (Niederlande) 
- Französisch  
- Deutsch 
- Italienisch (Italien) 
- Japanisch (Japan)  
- Portugiesisch (Brasilien) 
- Russisch (Russisch)  
- Spanisch 

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>Wie lange dauert es, bis die Website in unserer Mandanten Umgebung installiert wird?

Basierend auf den Tests der Installation sollte es weniger als 15 Minuten dauern. Dies umfasst nicht die Zeit, die erforderlich ist, um die Website auf Ihre Anforderungen anzupassen.

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Handelt es sich bei Microsoft 365-Lernpfaden um eine Open Source-Lösung, und welche Auswirkungen hat dies?

Microsoft 365 Lernpfade sind eine Open Source Software (OSS)-Lösung und tragen als solche eine Reihe von Vorteilen und Überlegungen für das deutsche für OSS:

#### <a name="benefits"></a>Vorzüge 
- **Microsoft 365 Lern Pfade ist eine ﻿kostenlose Lösung:** Kunden können die Lösung in Ihrem Mandanten installieren, anpassen und für Endbenutzer verfügbar machen.
- **OSS ermöglicht eine schnelle Entwicklung und Zusammenarbeit:**  Alle Open Source-Lösungen stehen einer breiten Community von Mitwirkenden zur Verfügung.  Microsoft setzt sich für diese Methode der Innovationssteuerung ein.  Um sicherzustellen, dass wir eine Erfahrung liefern, die den umfassendsten unserer Kunden zugute kommt, behält sich unser Kerndienst-Management-Team das Recht vor, festzustellen, welche Beiträge in unserem offiziellen Build zusammengeführt werden.  
- **OSS ermöglicht die Zusammenarbeit mit Partnern:** Microsoft arbeitet mit mehreren Lernpartnern zusammen, um Ihre Bemühungen für zukünftige Erweiterungen und Beiträge für Microsoft 365-Lern Pfade zu unterstützen. Wir werden weitere Informationen bereitstellen, wenn diese Pläne abgeschlossen werden. 
    
#### <a name="implications"></a>Auswirkungen
- **OSS ist kein kommerziell verfügbares Produkt:** Kommerzielle Produkte umfassen Aktualisierung und Patching und sind in gebührenbasierten Supportverträgen enthalten. Während Microsoft derzeit Dokumentation, Aktualisierung und Patchen für Microsoft 365-Lern Pfade anbietet, basiert es auf unserer Verpflichtung, dieses spezielle Geschäftsszenario zu verbessern. Unsere Pläne sind es, weiterhin in Lernpfade zu investieren, aber die Kunden sollten sich darüber im klaren sein, dass unser Service Management Team in Zukunft auch Strategien ändern kann. Zukünftige Änderungen an den Lernpfaden von Microsoft 365 werden vorab mitgeteilt, bevor Sie wirksam werden. 
- **Als OSS werden Microsoft 365-Lern Pfade über eine Online-Problemliste auf GitHub unterstützt**: Microsoft 365-Lernpfade werden nicht von einem vorhandenen Microsoft-Supportvertrag abgedeckt. Übermittelte Probleme werden von Microsoft 365-Dienstbesitzern und der Community für Lern Pfade für Bildungsgänge abgesprochen. Die Problem Auflösungsdienst Ebenen befinden sich nicht auf der gleichen Ebene wie ein bezahlter Microsoft-Supportvertrag.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>Können wir die Microsoft 365 Learning-Pfade zu einer Unterwebsite unserer primären SharePoint-Websitesammlung machen?

Nein. Die Website basiert auf einer Kommunikationswebsite Vorlage, die immer als Stammwebsitesammlung gedacht ist.

> [!NOTE]
> Es ist wichtig, die Berechtigungen zu beachten, die Ihre Endbenutzer für den Zugriff auf die Website benötigen. Die meisten Organisationen haben Sicherheits-oder Benutzergruppen definiert. Sie müssen dem neuen Schulungsportal die entsprechenden Sicherheitsgruppen hinzufügen, sobald Sie es für Ihre Mitarbeiter Community starten können.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>Ich muss die Website neu installieren; Was soll ich tun?

Befolgen Sie die [hier](custom_provision.md)veröffentlichten Installationsanweisungen.

> [!NOTE]
> Wenn Sie die Telemetrie in Ihrer vorherigen Installation deaktiviert haben und mit deaktivierter Telemetrie fortfahren möchten, müssen Sie die Anweisungen zum Deaktivieren der Telemetrie hier befolgen.

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Wir haben Updates für unsere Implementierung von Microsoft 365-Lernpfaden vorgenommen. Werden diese Updates (erstellt in der Websitevorlage, Wiedergabelisten) verloren, wenn wir die Website neu installieren?

Anpassungen für einzelne Seiten und benutzerdefinierte Wiedergabelisten gehen verloren, wenn Sie die Website über Ihre aktuelle Installation neu installieren.  