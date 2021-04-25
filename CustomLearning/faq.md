---
title: Häufig gestellte Fragen zu Microsoft 365-Lernpfaden
author: karuanag
ms.author: karuanag
ms.date: 02/10/2019
description: Häufig gestellte Fragen zu Microsoft 365-Lernpfaden
ms.service: sharepoint-online
ms.openlocfilehash: d91c2710315b393eb8be3645c4fa94b32d353aa7
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/25/2021
ms.locfileid: "52000081"
---
# <a name="frequently-asked-questions"></a>Häufig gestellte Fragen

### <a name="i-recently-saw-a-blog-post-that-custom-learning-for-office-365-is-being-renamed-to-microsoft-365-learning-pathways-are-there-other-changes-being-added-to-the-solution-as-part-of-the-renaming-effort-should-i-update-the-solution-in-my-organization"></a>Ich habe kürzlich einen Blogbeitrag gesehen, in dem Custom Learning für Office 365 in Microsoft 365-Lernpfade umbenannt wird. Werden der Lösung im Rahmen der Umbenennung weitere Änderungen hinzugefügt? Soll ich die Lösung in meiner Organisation aktualisieren?

Die Microsoft 365-Lernpfadeversion ist eine Umbranding-Anstrengung, um den Namen der Lösung so zu ändern, dass sie mit dem Microsoft 365-Branding in Einklang steht. Wenn Custom Learning für Office 365 derzeit erfolgreich in Ihrer Organisation ausgeführt wird, ist es derzeit nicht erforderlich, die Lösung zu aktualisieren.  

### <a name="what-are-the-requirements-for-installing-microsoft-365-learning-pathways-into-my-tenant-environment"></a>Welche Anforderungen gelten für die Installation von Microsoft 365-Lernpfaden in meiner Mandantenumgebung?

- SharePoint Online- und Kommunikationswebsites aktiviert.
- Die Person, die DENK365 bereitstellen wird, muss der Mandantenadministrator des Ziel-Mandanten für die Installation sein.
- Ein Mandant "App Catalog" muss innerhalb der Option "Apps" des SharePoint Admin Center verfügbar sein.
- Wenn ein neuer App-Katalog erstellt wird, ist eine Wartezeit von 30 Minuten oder mehr erforderlich, damit der App-Katalog vollständig bereitgestellt wird. Wenn Sie versuchen, Microsoft 365-Lernpfade direkt nach dem Erstellen des Mandanten-App-Katalogs bereitstellen, tritt ein Bereitstellungsfehler der Lösung für Lernpfade auf. 
- Die Person, die DENK365 bereitstellen soll, muss ein Websitesammlungsadministrator des App-Katalogs im Ziel-Mandanten für die Installation sein.

### <a name="why-is-microsoft-asking-for-tenant-permissions-when-installing-microsoft-365-learning-pathways"></a>Warum bittet Microsoft bei der Installation von Microsoft 365-Lernpfaden um Mandantenberechtigungen 

- Der SharePoint Online-Bereitstellungsdienst verwendet die Berechtigungen zum Bereitstellen der SharePoint-Website "Lernpfade", zum Erstellen der Seiten der Website und zum Installieren der Microsoft 365-Lernpfadanwendung in ihrem Mandanten. Dies ist der einzige Grund, warum wir die Berechtigungen anfordern. Ohne die angeforderten Berechtigungen kann der SharePoint-Bereitstellungsdienst die Befehle nicht ausführen, die die Websitevorlage und das Webteil für Lernpfade automatisch installieren. 

### <a name="what-are-the-implications-of-microsoft-365-learning-pathways-being-in-a-beta-preview"></a>Welche Auswirkungen hat eine Betavorschau auf Microsoft 365-Lernpfade? 

Microsoft 365-Lernpfade befindet sich derzeit in der Betavorschau. Berücksichtigen Sie folgendes, wenn Sie Microsoft 365-Lernpfade auswerten, planen und implementieren:

- Wie bei jeder Betalösung behält sich unser Serviceverwaltungsteam das Recht vor, Änderungen am Dienst und seinen Komponenten vorzunehmen. Da Sie Fehler und UX-Probleme aktiv beheben, müssen Sie das WebPart wahrscheinlich aktualisieren.
- Um das Webteil zu aktualisieren, müssen Sie es aus unserem GitHub-Repository herunterladen und in Ihren Mandanten-App-Katalog hochladen. Weitere Informationen finden Sie im Abschnitt "Aktualisieren der Lösung" der [Readme-Datei](https://github.com/pnp/custom-learning-office-365/blob/master/README.md) für Microsoft 365-Lernpfade. 

### <a name="what-languages-is-microsoft-365-learning-pathways-available-in"></a>In welchen Sprachen sind Microsoft 365-Lernpfade verfügbar?

Microsoft 365-Lernpfade sind derzeit nur in Englisch verfügbar. Die automatische End-to-End-Bereitstellung funktioniert nur mit englischen Mandanten. Wir planen, den mehrsprachigen Support für die folgenden Sprachen im zweiten Quartal 2020 zu bieten. 

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

### <a name="is-microsoft-365-learning-pathways-an-open-source-solution-and-what-are-the-implications"></a>Ist Microsoft 365-Lernpfade eine Open-Source-Lösung, und welche Auswirkungen hat dies?

Microsoft 365-Lernpfade sind eine Open-Source-Software (OSS)-Lösung, die eine Reihe von Vorteilen und Überlegungen für OSS mit sich bringt:

#### <a name="benefits"></a>Vorteile 
- **Microsoft 365-Lernpfade sind eine kostenlose Lösung:** Kunden können die Lösung in ihrem Mandanten installieren, anpassen und endbenutzern zur Verfügung stellen
- **OSS ermöglicht eine schnelle Entwicklung und Zusammenarbeit:**  Alle Open-Source-Lösungen stehen einer breiten Community von Mitwirkenden zur Verfügung.  Microsoft setzt sich für diese Methode zur Förderung von Innovationen ein.  Um sicherzustellen, dass wir eine Erfahrung bereitstellen, von der die breiteste Gruppe unserer Kunden profitiert, behält sich unser Kernteam für die Dienstverwaltung das Recht vor, zu bestimmen, welche Beiträge in unserem offiziellen Build zusammengeführt werden.  
- **OSS ermöglicht die Zusammenarbeit mit Partnern:** Microsoft arbeitet mit mehreren Lernpartnern zusammen, um ihre Bemühungen um zukünftige Erweiterungen und Beiträge zu Microsoft 365-Lernpfaden zu unterstützen. Wir werden weitere Informationen bereitstellen, sobald diese Pläne finalisiert werden. 
    
#### <a name="implications"></a>Implikationen
- **OSS ist kein kommerziell verfügbares Produkt:** Kommerzielle Produkte umfassen Aktualisierungen und Patching und sind in kostenpflichtigen Supportverträgen enthalten. Obwohl Microsoft derzeit Dokumentation, Aktualisierung und Patching für Microsoft 365-Lernpfade anbietet, basiert es auf unserer Verpflichtung, dieses bestimmte Geschäftsszenario zu verbessern. Unsere Pläne sind es, weiterhin in Lernpfade zu investieren, und beachten Sie, dass unser Servicemanagementteam in Zukunft Strategien ändern kann. Alle zukünftigen Änderungen an Microsoft 365-Lernpfaden werden vor dem Wirksam werden kommuniziert. 
- **Als OSS werden Microsoft 365-Lernpfade** über eine Onlineproblemeliste auf GitHub unterstützt: Microsoft 365-Lernpfade werden nicht von einem vorhandenen Microsoft-Supportvertrag abgedeckt. Übermittelte Probleme werden von Den Besitzern von Microsoft 365-Lernpfaden und der Community triagediert. Die Servicelevels für die Problembeauflösung befinden sich NICHT auf der gleichen Stufe wie ein kostenpflichtiger Microsoft-Supportvertrag.  

### <a name="can-we-make-the-microsoft-365-learning-pathways-a-subsite-of-our-primary-sharepoint-site-collection"></a>Können wir die Microsoft 365-Lernpfade zu einer Unterwebsite unserer primären SharePoint-Websitesammlung machen?

Nein. Die Website basiert auf einer Kommunikationswebsitevorlage, die immer als Stammwebsitesammlung gedacht ist.

> [!NOTE]
> Es ist wichtig, die Berechtigungen zu berücksichtigen, die Ihre Endbenutzer für den Zugriff auf die Website benötigen. Die meisten Organisationen haben Sicherheits- oder Benutzergruppen definiert. Sie müssen dem neuen Schulungsportal die entsprechenden Sicherheitsgruppen hinzufügen, sobald Sie bereit sind, es in Ihrer Mitarbeiter-Community zu starten.

### <a name="i-need-to-reinstall-the-site-what-should-i-do"></a>Ich muss die Website neu installieren. Was soll ich tun?

Befolgen Sie die hier veröffentlichten [Installationsanweisungen.](custom_provision.md)

> [!NOTE]
> Wenn Sie die Telemetrie in Ihrer vorherigen Installation deaktiviert haben und die Telemetrie deaktivieren möchten, müssen Sie hier die Anweisungen zum Deaktivieren der Telemetrie befolgen.

### <a name="we-made-updates-to-our-implementation-of-microsoft-365-learning-pathways-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a>Wir haben Updates für die Implementierung von Microsoft 365-Lernpfaden vorgenommen. Gehen diese Updates (an Websitevorlage, Wiedergabelisten) verloren, wenn wir die Website erneut installieren?

Anpassungen an einzelnen Seiten und benutzerdefinierten Wiedergabelisten gehen verloren, wenn Sie die Website über Die aktuelle Installation neu installieren.  
