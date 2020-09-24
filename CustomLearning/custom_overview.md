---
author: pkrebs
ms.author: pkrebs
title: Lernpfade anpassen
ms.date: 02/18/2019
description: Lernpfade anpassen
ms.service: sharepoint online
ms.openlocfilehash: 56027e48917cbdeeb2187f87497f3281fff3c23a
ms.sourcegitcommit: ee4aebf60893887ae95a1294a9ad8975539ea762
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/23/2020
ms.locfileid: "48234227"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="90207-103">Lernpfade anpassen</span><span class="sxs-lookup"><span data-stu-id="90207-103">Customize learning pathways</span></span>

<span data-ttu-id="90207-104">Microsoft 365-Lern Pfade bieten eine Vielzahl von Möglichkeiten, mit denen Sie Inhalte für Ihre Organisation anpassen können.</span><span class="sxs-lookup"><span data-stu-id="90207-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="90207-105">Beispielsweise können Sie folgende Aktionen ausführen:</span><span class="sxs-lookup"><span data-stu-id="90207-105">For example, you can:</span></span>  
- <span data-ttu-id="90207-106">Ändern der Lernpfade SharePoint-Website – ändern Sie den Websitenamen, das Logo und diese.</span><span class="sxs-lookup"><span data-stu-id="90207-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="90207-107">Ändern Sie die Seite Ask Questions und Get Help, um Ihre eigene Hilfe zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="90207-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="90207-108">Ausblenden oder Anzeigen von Inhalten, um die in Ihrer Organisation unterstützten Dienste oder Features widerzuspiegeln</span><span class="sxs-lookup"><span data-stu-id="90207-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="90207-109">Erstellen benutzerdefinierter Wiedergabelisten und Unterkategorien, die speziell für die Anforderungen Ihrer Benutzer erstellt wurden</span><span class="sxs-lookup"><span data-stu-id="90207-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="90207-110">Erstellen von Zielseiten mit gefiltertem Inhalt zur Unterstützung geschäftlicher Ergebnisse, beispielsweise das Vorantreiben der Einführung von Microsoft Teams, Outlook Mobile oder die Zusammenarbeit mit Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="90207-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![cg-introducing.png](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="90207-112">Anforderungen und Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="90207-112">Requirements and Permissions</span></span>

<span data-ttu-id="90207-113">Bevor Sie mit dem Leitfaden zum Anpassen von Lernpfaden beginnen, stellen Sie sicher, dass von Ihrem SharePoint-Mandanten Administrator Lern Pfade eingerichtet wurden.</span><span class="sxs-lookup"><span data-stu-id="90207-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="90207-114">Wenn Sie sich nicht sicher sind, ob Sie eingerichtet wurde, wenden Sie sich an Ihren SharePoint-mandantenadministrator, um zu überprüfen, ob Lern Pfade bereitgestellt wurden.</span><span class="sxs-lookup"><span data-stu-id="90207-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="90207-115">Stellen Sie außerdem sicher, dass Sie die URL der SharePoint-Website für Lern Pfade abrufen.</span><span class="sxs-lookup"><span data-stu-id="90207-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="90207-116">Wenn Sie der Mandanten Administrator sind und keine Lern Pfade eingerichtet wurden, finden Sie weitere Informationen unter [Bereitstellungspfade](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="90207-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="90207-117">Berechtigungen zur Vermittlung von Lernpfaden</span><span class="sxs-lookup"><span data-stu-id="90207-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="90207-118">Mandantenadministrator, auch bekannt als Office 365 globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="90207-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="90207-119">Der SharePoint-Websitesammlungsadministrator mit Besitzerberechtigungen für die Website</span><span class="sxs-lookup"><span data-stu-id="90207-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="90207-120">Berechtigungen zum Verwenden von Verwaltungsfeatures für Lern Pfade</span><span class="sxs-lookup"><span data-stu-id="90207-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="90207-121">Websitesammlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="90207-121">Site Collection Administrator</span></span>
- <span data-ttu-id="90207-122">SharePoint-Besitzer-oder Mitgliedsberechtigungen</span><span class="sxs-lookup"><span data-stu-id="90207-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="90207-123">Berechtigungen zum Verwenden der Website für Lern Pfade als Benutzer</span><span class="sxs-lookup"><span data-stu-id="90207-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="90207-124">Office 365-Benutzerberechtigungen/Berechtigungen für SharePoint-Websitebesucher oder höher</span><span class="sxs-lookup"><span data-stu-id="90207-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="90207-125">Erste Schritte der Anpassung</span><span class="sxs-lookup"><span data-stu-id="90207-125">Get started with customization</span></span>
<span data-ttu-id="90207-126">Nachdem Sie sichergestellt haben, dass Sie über die erforderlichen Berechtigungen zum Anpassen der Website und des Webparts verfügen, ist es an der Zeit, mit dem Anpassungsprozess begonnen zu werden.</span><span class="sxs-lookup"><span data-stu-id="90207-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="90207-127">Informationen zu den ersten Schritten finden Sie unter [Wechseln zur Website für Lern Pfade](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="90207-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>