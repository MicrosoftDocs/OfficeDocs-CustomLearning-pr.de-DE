---
title: Microsoft 365 Häufig gestellte Fragen zu Lernpfaden
author: karuanag
ms.author: karuanag
manager: alexb
ms.date: 02/10/2019
description: Häufig gestellte Fragen zu Microsoft 365 Lernpfaden
ms.service: sharepoint-online
ms.topic: article
ms.openlocfilehash: f24f16455ba41724d300d038a01dc04c2170dc4a
ms.sourcegitcommit: 33acfc2149de89e8375b064b2223cae505d2a102
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52575920"
---
# <a name="frequently-asked-questions"></a>Häufig gestellte Fragen

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>Ich habe kürzlich einen Blogbeitrag gesehen, in dem Custom Learning for Office 365 in Microsoft 365 umbenannt wird. Werden der Lösung im Rahmen der Umbenennung weitere Änderungen hinzugefügt? Soll ich die Lösung in meiner Organisation aktualisieren?

Die Microsoft 365 der Lernpfade ist eine Umbranding-Anstrengung, um den Namen der Lösung so zu ändern, dass sie Microsoft 365 wird. Wenn Custom Learning for Office 365 in Ihrer Organisation erfolgreich ausgeführt wird, ist es derzeit nicht erforderlich, die Lösung zu aktualisieren.  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>Welche Anforderungen gelten für die Installation Microsoft 365 Lernpfade in meiner Mandantenumgebung?

- SharePoint Online- und Kommunikationswebsites aktiviert.
- Die Person, die DENK365 bereitstellen wird, muss der Mandantenadministrator des Ziel-Mandanten für die Installation sein.
- Ein Mandant "App Catalog" muss innerhalb der Option "Apps" des SharePoint Admin Center verfügbar sein.
- Wenn ein neuer App-Katalog erstellt wird, ist eine Wartezeit von 30 Minuten oder mehr erforderlich, damit der App-Katalog vollständig bereitgestellt wird. Der Versuch, Microsoft 365 Lernpfade direkt nach dem Erstellen des Mandanten-App-Katalogs bereitstellen, führt zu einem Bereitstellungsfehler der Lösung für Lernpfade. 
- Die Person, die DENK365 bereitstellen soll, muss ein Websitesammlungsadministrator des App-Katalogs im Ziel-Mandanten für die Installation sein.

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Warum fordert Microsoft Mandantenberechtigungen bei der Installation Microsoft 365 Lernpfade an? 

- Der SharePoint Onlinebereitstellungsdienst verwendet die Berechtigungen zum Bereitstellen der Lernpfade SharePoint-Website, zum Erstellen der Seiten der Website und zum Installieren der Microsoft 365-Lernpfadanwendung innerhalb ihres Mandanten. Dies ist der einzige Grund, warum wir die Berechtigungen anfordern. Ohne die angeforderten Berechtigungen kann SharePoint Bereitstellungsdienst die Befehle nicht ausführen, die die Websitevorlage und das Webteil für Lernpfade automatisch installieren. 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>Welche Auswirkungen hat Microsoft 365 lernpfade in einer Betavorschau? 

Microsoft 365 Lernpfade befindet sich derzeit in der Betavorschau. Berücksichtigen Sie folgendes, wenn Sie Lernpfade Microsoft 365 auswerten, planen und implementieren:

- Wie bei jeder Betalösung behält sich unser Serviceverwaltungsteam das Recht vor, Änderungen am Dienst und seinen Komponenten vorzunehmen. Da Sie Fehler und UX-Probleme aktiv beheben, müssen Sie das WebPart wahrscheinlich aktualisieren.
- Um das Webteil zu aktualisieren, müssen Sie es aus unserem GitHub-Repository herunterladen und in Ihren Mandanten-App-Katalog hochladen. Lesen Sie den Abschnitt "Aktualisieren der Lösung" der Microsoft 365 [Readme-Datei](https://github.com/pnp/custom-learning-office-365/blob/master/README.md) für Lernpfade. 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>In welchen Sprachen Microsoft 365 lernpfade verfügbar?

Microsoft 365 Lernpfade sind derzeit nur in Englisch verfügbar. Die automatische End-to-End-Bereitstellung funktioniert nur mit englischen Mandanten. Wir planen, den mehrsprachigen Support für die folgenden Sprachen im zweiten Quartal 2020 zu bieten. 

- Chinesisch (vereinfacht) 
- Französisch  
- Deutsch 
- Italienisch (Italien) 
- Japanisch (Japan)  
- Portugiesisch (Brasilien) 
- Russisch (Russisch)  
- Spanisch 

> Unterstützung für die niederländische Sprache wird in der bevorstehenden Veröffentlichung der mehrsprachigen Unterstützung für Lernpfade nicht enthalten sein. Wir werden auch in Zukunft neue Sprachoptionen auswerten.

### <a name="how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a>Wie lange dauert die Installation der Website in unserer Mandantenumgebung?

Basierend auf unseren Tests der Installation sollte es weniger als 15 Minuten dauern. Dies schließt nicht die Zeit ein, die für die Anpassung der Website an Ihre Anforderungen erforderlich ist.

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Ist Microsoft 365 Lernpfade eine Open-Source-Lösung, und welche Auswirkungen hat dies?

Microsoft 365 Lernpfade ist eine Open Source Software (OSS)-Lösung und bietet als solche eine Reihe von Vorteilen und Überlegungen für OSS:

#### <a name="benefits"></a>Vorteile 
- **Microsoft 365 Lernpfade ist eine kostenlose Lösung:** Kunden können die Lösung in ihrem Mandanten installieren, anpassen und endbenutzern zur Verfügung stellen
- **OSS ermöglicht eine schnelle Entwicklung und Zusammenarbeit:**  Alle Open-Source-Lösungen stehen einer breiten Community von Mitwirkenden zur Verfügung.  Microsoft setzt sich für diese Methode zur Förderung von Innovationen ein.  Um sicherzustellen, dass wir eine Erfahrung bereitstellen, von der die breiteste Gruppe unserer Kunden profitiert, behält sich unser Kernteam für die Dienstverwaltung das Recht vor, zu bestimmen, welche Beiträge in unserem offiziellen Build zusammengeführt werden.  
- **OSS ermöglicht die Zusammenarbeit mit Partnern:** Microsoft arbeitet mit mehreren Lernpartnern zusammen, um ihre Bemühungen um zukünftige Erweiterungen und Beiträge für Microsoft 365 zu unterstützen. Wir werden weitere Informationen bereitstellen, sobald diese Pläne finalisiert werden. 
    
#### <a name="implications"></a>Implikationen
- **OSS ist kein kommerziell verfügbares Produkt:** Kommerzielle Produkte umfassen Aktualisierungen und Patching und sind in kostenpflichtigen Supportverträgen enthalten. Obwohl Microsoft derzeit Dokumentation, Aktualisierung und Patching für Microsoft 365 bietet, basiert es auf unserem Engagement für die Verbesserung dieses bestimmten Geschäftsszenarios. Unsere Pläne sind es, weiterhin in Lernpfade zu investieren, und beachten Sie, dass unser Servicemanagementteam in Zukunft Strategien ändern kann. Alle zukünftigen Änderungen Microsoft 365 Lernpfaden werden vor dem Wirksam werden kommuniziert. 
- **Als OSS werden Microsoft 365** Lernpfade über eine Online-Problemliste unter GitHub unterstützt: Microsoft 365 Lernpfade werden nicht durch einen vorhandenen Microsoft-Supportvertrag abgedeckt. Übermittelte Probleme werden von den Microsoft 365 und der Community triagediert. Die Servicelevels für die Problembeauflösung befinden sich NICHT auf der gleichen Stufe wie ein kostenpflichtiger Microsoft-Supportvertrag.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>Können wir die Microsoft 365 lernpfade zu einer Unterwebsite unserer primären SharePoint machen?

Nein. Die Website basiert auf einer Kommunikationswebsitevorlage, die immer als Stammwebsitesammlung gedacht ist.

> [!NOTE]
> Es ist wichtig, die Berechtigungen zu berücksichtigen, die Ihre Endbenutzer für den Zugriff auf die Website benötigen. Die meisten Organisationen haben Sicherheits- oder Benutzergruppen definiert. Sie müssen dem neuen Schulungsportal die entsprechenden Sicherheitsgruppen hinzufügen, sobald Sie bereit sind, es in Ihrer Mitarbeiter-Community zu starten.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>Ich muss die Website neu installieren. Was soll ich tun?

Befolgen Sie die hier veröffentlichten [Installationsanweisungen.](custom_provision.md)

> [!NOTE]
> Wenn Sie die Telemetrie in Ihrer vorherigen Installation deaktiviert haben und die Telemetrie deaktivieren möchten, müssen Sie hier die Anweisungen zum Deaktivieren der Telemetrie befolgen.

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Wir haben die Implementierung von lernpfaden Microsoft 365 aktualisiert. Gehen diese Updates (an Websitevorlage, Wiedergabelisten) verloren, wenn wir die Website erneut installieren?

Anpassungen an einzelnen Seiten und benutzerdefinierten Wiedergabelisten gehen verloren, wenn Sie die Website über Die aktuelle Installation neu installieren.  
