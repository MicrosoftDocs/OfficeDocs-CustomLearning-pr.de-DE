---
author: pkrebs
ms.author: pkrebs
title: Partner-Integrationsmodelle
ms.date: 3/9/2019
description: Partner-Integrationsmodelle
ms.service: sharepoint online
ms.openlocfilehash: f3b5c5ddc8de29d2805c86a24b1d9bef0c8cacfa
ms.sourcegitcommit: 907c657e7cc5a4a44d2b9f38cc35fea9ac5c5943
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2021
ms.locfileid: "51162932"
---
# <a name="partner-integration-models"></a>Partner-Integrationsmodelle
Es ist zwar nicht möglich, die Inhalte von Microsoft 365-Lernpfaden direkt "sofort" über den SharePoint Online-Bereitstellungsdienst zu ergänzen, es gibt jedoch mehrere Integrationsmodelle, die Partner nutzen können, um ausgerichtete Mehrwertdienstangebote zu erstellen. Die oben genannten Partnerintegrationsmodelle werden in der Reihenfolge der aufsteigenden Komplexität und der Höhe der Investitionen dargestellt. Daher ist es unsere Anleitung, Ihr Fachwissen zu entwickeln und auf anspruchsvollere Ebenen basierend auf Ihren Geschäftsmodellen zu graduierten.

![cg-part-intmodel.png](media/cg-part-intmodel.png) 

## <a name="how-should-i-get-started"></a>Wie soll ich beginnen? 
In den ersten Schritte finden Sie einige bewährte Methoden, die Sie befolgen sollten.     

### <a name="1-begin-with-building-expertise-as-an-enabler"></a>1. Beginnen Sie mit dem Erstellen von Fachwissen als Enabler. 
Sie können einen Prozentsatz Ihrer Kundenbasis sofort unterstützen, indem Sie ihr Schulungsportal für Lernpfade aktivieren und eine gezielte Microsoft-Inhaltskuration durchführen. Anweisungen zur Bereitstellung von Lernpfaden finden Sie unter https://docs.microsoft.com/office365/customlearning/custom_provision .  

### <a name="2-then-extend-your-services-as-an-integrator"></a>2. Erweitern Sie dann Ihre Dienste als Integrator
Führen Sie eine Automatisierungsrendite bei der Investitionsanalyse durch – abhängig von der Menge Ihrer Anforderungen an die Inhalts- und/oder Dienstintegration. Beispielsweise ist es möglicherweise nicht sinnvoll, die Entwicklungs- und Betriebskosten im Hinblick auf unsere Richtlinien für die Inhaltsintegration zu übernehmen, wenn Sie schnell manuell eine gezielte benutzerdefinierte Wiedergabeliste erstellen können, die auf Ihre bezahlten Inhalte zeigt oder auf Ihre Dienste verweisen.

### <a name="3-when-the-return-on-investment-makes-sense--consider-redistribution"></a>3. Wenn die Rendite sinnvoll ist – Umverteilung in Betracht ziehen 
Wenn die Rendite sinnvoll ist – erwägen Sie die Umverteilung (oder die Zusammenarbeit mit verwandten Lernpfadpartnern), um umgepackte Lösungen zu erstellen. Diese basieren auf dem SharePoint Patterns and Practice-Framework, das Lösungen zum Extrahieren angepasster Websites und anschließender Bereitstellung in Kundenumgebungen bietet. 

## <a name="partner-provided-content-integration-guidelines"></a>Vom Partner bereitgestellte Richtlinien für die Inhaltsintegration
Inhalte für Microsoft 365-Lernpfade werden von einer Reihe von JSON-Dateien gesteuert, die als Inhaltsmanifesten für Ihr Lernpaket fungieren. Es gibt drei Dateien: metadata.js, playlists.jsund assets.js. Diese Dateien müssen so strukturiert sein, dass sie mit den Modellen übereinstimmen, die das Webteil erkennt und dann von einem Inhaltszustellungsnetzwerk (Content Delivery Network, CDN) gehostet wird, damit das Webteil sie laden kann. Microsoft stellt Startvorlagen dieser Dateien bereit, damit Sie beginnen können.  

**Haftungsausschluss:** Die Dateistruktur von JSON kann basierend auf anstehenden Lösungsarbeiten geändert werden. Der Microsoft 365-Lernpfadpartner Early Adopter Program (EAP) wird über bevorstehende Änderungen dieser Art informiert. Zusammen mit allen Abwärtskompatibilitäts- und/oder Übergangsanleitungen für Kunden. 

### <a name="download-the-microsoft-365-learning-pathways-solution"></a>Herunterladen der Microsoft 365-Lernpfadlösung
Sie können die Microsoft 365-Lernpfadlösung zusammen mit den JSON-Dateien aus dem GitHub-Repository herunterladen: https://github.com/pnp/custom-learning-office-365 . Beachten Sie, dass Microsoft derzeit keine GitHub-Pullanforderung für die Lösung verwendet. Sie können die GitHub-Dateien jedoch als Ausgangspunkt für die Erstellung Ihres eigenen benutzerdefinierten Inhaltspakets verwenden. 

### <a name="metadatajson-structure"></a>Metadata.jsauf Struktur
Sie können sich diese Datei als den Kopf der Menüs und der Struktur denken. Sie enthält alle Navigationsstrukturen sowie Auswahllisten für Daten in den anderen beiden Dateien. 


|              Name        |                     Beschreibung                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|**Technologien**              |Inhalte werden markiert und können basierend auf der zugewiesenen Technologie ausgeblendet werden.                 |  
|&nbsp;&nbsp;ID                |GUID, die die Technologie darstellt                                                           |  
|&nbsp;&nbsp;Name              |Anzeigename der Technologie                                                             |
|&nbsp;&nbsp;*Subjects[ ]*     |Ein Array von Probanden, die eine Teilmenge der Technologie sind                                   | 
|&nbsp;&nbsp;&nbsp;&nbsp;ID    |GUID, die den Betreff darstellt                                                              |
|&nbsp;&nbsp;&nbsp;&nbsp;Name  |Anzeigename des Betreffs                                                                |
|**Kategorien [ ]**             |Kategorien informieren die Navigation des Webparts. Jede Kategorie stellt eine oberste Ebene der Navigation dar.                                                                                                                 |
|&nbsp;&nbsp;ID                |GUID, die die Kategorie/Unterkategorie darstellt                                                 |
|&nbsp;&nbsp;Name              |Anzeigename für die Kategorie/Unterkategorie                                                  |
|&nbsp;&nbsp;Bild             |URL für das Bild, das in der UX angezeigt werden soll (relativ zur CDN-Basis)            |
|&nbsp;&nbsp;TechnologyId      |Die GUID der Technologie, mit der dieser Inhalt verknüpft ist (optional – leere Zeichenfolge)            |
|&nbsp;&nbsp;SubjectId         |Die GUID des Betreffs, mit dem dieser Inhalt verknüpft ist (optional – leere Zeichenfolge)               |
|&nbsp;&nbsp;Source            |Aus dem Source-Array, das nicht speziell in der UX verwendet wird, werden keine benutzerdefinierten Daten, die vom Benutzer hinzugefügt werden, als "Mandant" markiert, und der UX-Administratorbereich lässt die Bearbeitung von nichts zu, das nicht als "Mandant" gekennzeichnet ist.                           |
|&nbsp;&nbsp;*Unterkategorien[ ]*|Sub-Categories sind im Wesentlichen die Navigationsebene von Ebene 2 nach unten. Die Struktur ist identisch mit einer Kategorie, die gerade geschachtelt ist.          |
|**Zielgruppen [ ]**             |Wenn Wiedergabelisten, die einer Kategorie/Unterkategorie zugeordnet sind, verschiedenen Zielgruppen zugeordnet sind, steht eine Auswahl zur Verfügung, um die verfügbaren Benutzergruppen zu zeigen. |         
|&nbsp;&nbsp;ID                |GUID der Zielgruppe                                                                       |  
|&nbsp;&nbsp;Name              |Anzeigename der Zielgruppe                                                               |       
|**Quellen [ ]**               |Array von Zeichenfolgen, die Inhalte mit ihrer Quelle kennzeichnen, die nicht speziell in der UX verwendet werden, die nicht vom Benutzer hinzugefügte benutzerdefinierte Daten sind als "Mandant" gekennzeichnet, und der UX-Administratorbereich lässt die Bearbeitung von nicht als "Mandant" markierten Inhalten nicht zu.                                                   |  
|**Ebenen [ ]**               |Wenn wiedergabelisten, die einer Kategorie/Unterkategorie zugeordnet sind, verschiedene Ebenen sind, die markiert sind, steht eine Auswahl zur Verfügung, um die verfügbaren Ebenen zu zeigen.             |  
|&nbsp;&nbsp;ID                |GUID der Ebene                                                                          |  
|&nbsp;&nbsp;Name              |Anzeigename der Ebene                                                                  | 
|**StatusTag [ ]**           |Statustag ist das Identifizieren von Inhalten mit unterschiedlichen Status, die in der UX verfügbar gemacht werden. Einige dieser Kennzeichen werden dem Verbraucher und einige nur dem Administrator gezeigt.                                                   |  
|&nbsp;&nbsp;ID                |GUID des StatugTag                                                                      |  
|&nbsp;&nbsp;Name              |Anzeigename des StatusTags                                                              | 
|**Telemetrie [ ]**            |                                                                                           |  
|&nbsp;&nbsp;AppInsightsKey    |GUID des App-Insights-Schlüssels, den Sie zum Nachverfolgen des Ladens des Viewer-Web teils eingerichtet haben. Die Nachverfolgung kann von einem Administrator für den gesamten Mandanten deaktiviert werden, die gesendeten Informationen werden jedoch vom Benutzer mit der Mandanten-ID anonymisiert. Weitere Informationen finden Sie in diesem Abschnitt. https://github.com/pnp/custom-learning-office-365#disabling-telemetry-collection               |  
|**Version**                   |Versionsinformationen werden von der Lösung verwendet, um Administratoren anzuzeigen, dass das Webpart aktualisiert wurde, und es dem Webpart auch zu ermöglichen, benutzerdefinierte Inhalte auf die neueste Version des Manifests selbst zu aktualisieren, wenn wesentliche Änderungen vorgenommen wurden.         | 
|&nbsp;&nbsp;Manifest          |Die Version des Manifests                                               |
|&nbsp;&nbsp;ManifestMinWebPart|Die Mindestversion des Webparts, das mit der Version des Manifests funktioniert             |
|&nbsp;&nbsp;CurrentWebPart    |URL für das Bild, das in der UX angezeigt werden soll (relativ zur CDN-Basis)            |
|&nbsp;&nbsp;RepoURL           |Die URL des Repositorys, in dem die Anweisungen zum Aktualisieren des Webteils enthalten sind.                    |
|**Inhaltspakete**             |Inhaltspakete für zusätzliche CDNs werden derzeit nicht unterstützt. Mit Inhaltspaketen kann Microsoft andere von Microsoft erstellte Lösungen vorschlagen, die über den Bereitstellungsdienst bereitgestellt werden können, die M365LP zum Bereitstellen von Inhalten nutzen und sich in benutzerdefinierten CDNs befinden.       | 
|&nbsp;&nbsp;ID                |GUID des Inhaltspakets/CDN                                                              |
|&nbsp;&nbsp;Name              |Anzeigename des CDN                                                                   |
|&nbsp;&nbsp;Beschreibung       |Beschreibung, die auf der Benutzeroberfläche zum Hinzufügen eines Inhaltspakets angezeigt werden soll                               |
|&nbsp;&nbsp;Bild             |Bild, das in der Benutzeroberfläche zum Hinzufügen eines Inhaltspakets angezeigt werden soll                                     |
|&nbsp;&nbsp;ProvisionURL      |Die URL zum Bereitstellungsdienstpaket zum Erstellen der Websitesammlung des Inhaltspakets  |
|&nbsp;&nbsp;CDNbase           |Die Basis-URL für die Manifeste für das Inhaltspaket                                       |
|AssetOrigins                  |Ein Array mit URL-Ursprung, das in der Datei verwendet wird, assets.jsspäter beschrieben wird. Wenn die Ursprungs-URL sie unterstützt, wird eine Postnachricht an help_getClientHeight. Eine Antwort in der Dateneigenschaft von: "help_getClientHeight={Höhe des Inhalts}" (z. B. "help_getClientHeight=5769") ermöglicht es, die Größe des iFrames auf die entsprechende Höhe des gerahmten Inhalts zu ändern.         |

### <a name="playlistsjson-structure"></a>Playlists.jsauf Struktur
playlists.json – Das Wiedergabelistenmanifest ist ein Array von Objekten, die die Metadaten zu einer Wiedergabeliste und den In der Wiedergabeliste enthaltenen Ressourcen beschreiben.

|              Name        |                     Beschreibung                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|Id                            |GUID, die die Wiedergabeliste darstellt                                                             |  
|Titel                         |Anzeigename der Wiedergabeliste                                                               |
|Bild                         |Relative URL (vom CDN) zu einem Bild zum Visualisieren der Wiedergabeliste                              |                      
|LevelId                       |Zugeordnete Ebene                                                                           |
|AudienceId                   |Zugeordnete Zielgruppe                                                                        |
|TechnologyId                 |Zugehörige Technologie                                                                      |
|SubjectId                    |Anzeigename für die Kategorie/Unterkategorie                                                  |
|Source                        |Aus dem Quellarray, das nicht speziell in der UX verwendet wird, werden keine benutzerdefinierten Daten, die vom Benutzer hinzugefügt werden, als "Mandant" markiert, und der UX-Administratorbereich lässt die Bearbeitung von nichts zu, das nicht als "Mandant" gekennzeichnet ist.                                              |
|CatId                         |Die Category- oder SubCategory-ID, die den Container darstellt, in dem die Wiedergabeliste angezeigt werden soll. Derzeit unterstützt das Manifest die Auswahl einer Kategorie oder Unterkategorie als Container nicht, wenn es auch untergeordnete Unterkategorien enthält.        |
|Beschreibung                   |Eine Beschreibung, die für jede Wiedergabeliste in der UX angezeigt wird                                           |
|StatusTagId                   |Zugeordnetes Statustag                                                                      |
|StatusNote                    |Hinweise zu Inhalten, die Administratoren angezeigt werden                                            |
|*Assets[]*                        |Ein Array von GUID für die Objekte, die Teil dieser Wiedergabeliste sind, in der Anzeigereihenfolge.        |         

### <a name="assetjson-structure"></a>Asset.jsauf Struktur
playlists.json – Das Wiedergabelistenmanifest ist ein Array von Objekten, die die Metadaten zu einer Wiedergabeliste und den In der Wiedergabeliste enthaltenen Ressourcen beschreiben.

|              Name        |                     Beschreibung                                                               | 
|:-----------------------------|-------------------------------------------------------------------------------------------|
|Id                            |GUID, die die Wiedergabeliste darstellt                                                             |  
|Titel                         |Anzeigename der Wiedergabeliste                                                               |
|Beschreibung                   |---                                                                                           |                      
|URL                           |Die Quell-URL für die Ressource, die auf den iFrame angewendet werden soll                                  |
|TechnologyId                  |Zugehörige Technologie                                                                      |
|SubjectId                     |Zugeordneter Betreff                                                                         |
|Source                        |Anzeigename für die Kategorie/Unterkategorie                                                  |
|StatusTagId                   |Zugeordnetes Statustag                                                                      |
|StatusNote                    |Hinweise zu Inhalten, die Administratoren angezeigt werden.                                           |

### <a name="caching"></a>Zwischenspeicherung
Die aktuelle Version des Viewer-Web teils verwendet eine zwischengespeicherte Version der Manifestdateien für 24 Stunden. Nach 24 Stunden nutzt der erste Benutzer, der das Webpart getroffen hat, den Leistungstreffer, um den Cache zu aktualisieren, indem die Manifeste aus dem Quell-CDN heruntergeladen und diese Informationen mit ausgeblendeten Technologien und Wiedergabelisten zusammengeführt und in benutzerdefinierten Unterkategorien, Wiedergabelisten und Ressourcen zusammengeführt werden. Alternativ lädt das Administratorwebteil den Inhalt immer aus den Manifesten herunter, führt sie zusammen und aktualisiert den Cache.  Mit anderen Worten, der Administrator kann ein Cacheupdate jederzeit erzwingen, indem er das Administratorwebteil lädt, das auch zur Verwaltungsseite geht.

## <a name="content-pack-guidelines"></a>Richtlinien für Inhaltspaket
Das Content Pack-Feature entsperrt die folgenden Szenarien:
- Die Möglichkeit für Partner, mehrwertig angepasste benutzerdefinierte Lerninhalte weiterzuverteilen, die auf die Umgebung von Kunden zugeschnitten sind
- Die Möglichkeit für Organisationen mit einem starken Schulungsteam und IT-Unterstützung, benutzerdefinierte Lerninhalte zu erstellen, die auf ihre eigenen internen Systeme und Governance ausgerichtet sind
- Die Möglichkeit für Microsoft, in Zukunft zusätzliche Lernpfade zu bieten, für die Kunden sich entscheiden können

Dieser aktuelle Dokumentationssatz ist aufgrund der Komplexität des Features absichtlich auf Partner ausgerichtet. Das Serviceteam arbeitet aktiv an einer besseren Unterstützung und Aktivierung #2 Szenarios. 

### <a name="how-content-packs-work"></a>Funktionsweise von Inhaltspaketen
Microsoft verwendet GitHub-Seiten als Quelle für das Inhaltszustellungsnetzwerk (Content Delivery Network, CDN) für seine Manifestdateien und -bilder. Im Stammverzeichnis unseres GitHub-Repositorys befindet sich ein Docs-Ordner, der Unterordner für jede Version der Manifestdateien enthält. In jedem Ordner befinden sich drei Manifestdateien sowie ein Bilderordner zum Speichern aller Kategorie-, Unterkategorie- und Wiedergabelistenbilder. 

Es ist wichtig, dass Sie dieselbe Versionsstruktur wie Microsoft beibehalten, wenn Sie die Lösung für Lernpfade mit Ihrem eigenen Inhaltspaket erweitern möchten. Ihr CDN-Endpunkt sollte den Versionsordner nicht enthalten, da die vom Web part unterstützte Manifestversion in ihn eingebacken wird und automatisch an die CDN-URL angefügt wird. Wir geben Ihnen bei jeder Überarbeitung natürlich Zeit, neue Instanzen Ihrer Manifestdateien zu erstellen.

![cg-part-json-folder.png](media/cg-part-json-folder.png) 

Weitere Informationen zur Verwendung von GitHub-Seiten als CDN-Quelle finden Sie in der folgenden Hilfedokumentation: [https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages](https://help.github.com/en/articles/configuring-a-publishing-source-for-github-pages) .

Die Lösung von Microsoft macht die Informationen zu den Ressourcen für die Öffentlichkeit zugänglich, da es keine Sicherheit gibt, wer Zugriff auf diese Dateien hat. Wir sind der Meinung, dass es eine kostenlose Ebene von Inhalten für einen Verbraucher geben sollte, d. h. wenn Sie für einen Teil oder alle Inhalte eine Lohnwand benötigen, müssen Sie dies innerhalb der technischen Einschränkungen der Lösung anders implementieren und die Verwendung von GitHub-Seiten ist keinesfalls erforderlich. Jeder cdN-Anbieter, den Sie verwenden möchten, ist in Ordnung, wenn Sie die von uns beschriebene Versionsnummerierungsstruktur beibehalten. Wie bereits erwähnt, wird die Version der Manifeststruktur, die vom Web part unterstützt wird, in den Code gebacken und automatisch an die CDN-URL angefügt. 

### <a name="content-pack-integration-guidance"></a>Anleitung zur Inhaltspaketintegration 
Die Admin- und Viewer-Webparts wurden erweitert, um es dem Verbraucher zu ermöglichen, zusätzliche CDN-Endpunkte in ihrem Mandanten zu konfigurieren, wodurch das Viewerwebparts auswählen kann, welches CDN die angezeigten Daten quellen soll. 

Schlüsselrahmen, die für dieses Feature zu beachten sind: 
- Dies gilt vor allem für Partnerumverteilungsszenarien – bei denen die manuelle Wiedergabelistenkonfiguration zu umständlich ist 
- Benutzerdefinierte Inhaltspakete sind ein erweitertes Feature und sollten nur von Partnern mit Erfahrung bei der Verwaltung von Webinhalten verwendet werden. Nicht vertrauenswürdige Inhaltsquellen führen möglicherweise zu unsicheren Inhalten auf Ihrer Website. Sie sollten nur Quellen hinzufügen, die Sie vertrauenswürdig sind.

> **WICHTIG** Vor dem Hinzufügen eines benutzerdefinierten Inhaltspakets müssen Sie Microsoft 365-Lernpfade 3.0 oder höher bereitgestellt haben. Informationen zur Bereitstellung von Microsoft 365-Lernpfaden finden Sie unter [Provision Microsoft 365 learning pathways](./custom_provision.md).

### <a name="content-whitelisting"></a>Whitelisting für Inhalte
Als Partner liegt es in Ihrer Verantwortung, Ihren Kunden dabei zu helfen, sicherzustellen, dass Ihre Inhalte in ihrer Umgebung auf die Whitelist gesetzt sind. Wir empfehlen Ihnen, ein Testszenario in ihrer Umgebung zu erstellen, um zu überprüfen, ob Ihre Inhalte iFrame'd in einer SharePoint-Seite innerhalb ihrer Firewall sein können. Befolgen Sie [die Anweisungen zum Erstellen von SharePoint-Seiten für benutzerdefinierte Wiedergabelisten,](./custom_createnewpage.md) um zu bestätigen, dass dies der Fall ist.

### <a name="add-a-content-pack-to-learning-pathways"></a>Hinzufügen eines Inhaltspakets zu Lernpfaden
Nachdem Sie das JSON erstellt und Ihr CDN definiert haben, können Sie das Contact Pack zu Lernpfaden hinzufügen. 

1. Zeigen Sie auf  der Startseite der Lernpfadewebsite auf **Home,** und klicken Sie dann auf **Verwaltung von Lernpfaden.** 
2. Klicken Sie **auf der Seite** Verwaltung auf die Schaltfläche **... Fügen Sie Content Pack** in der oberen rechten Ecke der Seite hinzu.
3. Klicken Sie auf Benutzerdefiniertes Inhaltspaket, und geben Sie dann einen Namen des Inhaltspakets ein, und geben Sie dann den CDN an, in dem sich die JSON-Dateien befinden.

![cg-part-addconpack.png](media/cg-part-addconpack.png)

4. Klicken Sie auf **Speichern**. Der Inhalt ihres benutzerdefinierten Inhaltspakets sollte nun auf der Seite Verwaltung angezeigt werden. Hier ein Beispiel. 

![cg-part-addconpackex.png](media/cg-part-addconpackex.png)

### <a name="filter-to-the-content-pack-in-the-web-part"></a>Filtern in das Inhaltspaket im Webteil
Mit Lernpfaden können Sie das Web part für Lernpfade zu einer Seite hinzufügen, das Webteil filtern, um auf die Benutzerdefinierte Inhaltspaketquelle zu verweisen, und dann das Webteil nach der Kategorie, Unterkategorie, Wiedergabeliste und dem Objekt filtern, die Sie möchten. 

1. Klicken Sie auf der Lernpfadwebsite auf **Neu** und dann **auf Seite**.
2. Klicken **Sie auf Leer,** und erstellen **Sie dann Seite**.
3. Geben Sie der Seite einen Namen. 
4. Klicken **Sie auf der linken Seite** der Seite auf + Hinzufügen eines neuen Abschnitts.
5. Klicken Sie in der oberen Mitte des neuen Abschnitts, und fügen Sie dann das **+** **Microsoft 365-Lernpfadwebteil** hinzu.
6. Klicken Sie auf das Webteil, und klicken Sie dann auf das **Symbol Bearbeiten.**
7. Wählen Sie **im Feld Lernquelle** auswählen Das benutzerdefinierte Inhaltspaket aus, und filtern Sie das Webteil nach dem inhalt, den Sie möchten. Im Folgenden finden Sie ein Beispiel für das Webteil, das aus einem benutzerdefinierten Inhaltspaket in eine Wiedergabeliste gefiltert wurde.

![cg-part-conpackfilter.png](media/cg-part-conpackfilter.png)