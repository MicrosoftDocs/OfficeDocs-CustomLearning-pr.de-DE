---
author: pkrebs
ms.author: pkrebs
title: Lernpfade anpassen
ms.date: 02/18/2019
manager: bpardi
audience: admin
ms.topic: article
description: Lernpfade anpassen
ms.service: sharepoint-online
ms.openlocfilehash: a5087096ec3bd7c1194aab9dd089276fc196a736
ms.sourcegitcommit: 97e175e5ff5b6a9e0274d5ec9b39fdf7e18eb387
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/25/2021
ms.locfileid: "51999501"
---
# <a name="customize-learning-pathways"></a><span data-ttu-id="f7dc0-103">Lernpfade anpassen</span><span class="sxs-lookup"><span data-stu-id="f7dc0-103">Customize learning pathways</span></span>

<span data-ttu-id="f7dc0-104">Microsoft 365-Lernpfade bieten eine Vielzahl von Möglichkeiten zum Anpassen von Inhalten für Ihre Organisation.</span><span class="sxs-lookup"><span data-stu-id="f7dc0-104">Microsoft 365 learning pathways provides a variety of ways that you can customize content for your organization.</span></span> <span data-ttu-id="f7dc0-105">Beispielsweise können Sie folgende Aktionen ausführen:</span><span class="sxs-lookup"><span data-stu-id="f7dc0-105">For example, you can:</span></span>  
- <span data-ttu-id="f7dc0-106">Ändern der SharePoint-Lernpfade – Ändern des Websitenamens, des Logos und dieser.</span><span class="sxs-lookup"><span data-stu-id="f7dc0-106">Modify the learning pathways SharePoint site - Change the site name, logo, and them.</span></span> <span data-ttu-id="f7dc0-107">Ändern Sie die Seite Fragen stellen und Hilfe erhalten, um Ein eigenes Hilfecenter zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="f7dc0-107">Modify the Ask Questions and Get Help page to create your own Help Center.</span></span> 
- <span data-ttu-id="f7dc0-108">Ausblenden oder Anzeigen von Inhalten zur Widerspiegelung der in Ihrer Organisation unterstützten Dienste oder Features</span><span class="sxs-lookup"><span data-stu-id="f7dc0-108">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="f7dc0-109">Erstellen benutzerdefinierter Wiedergabelisten und Unterkategorien, die speziell für die Anforderungen Ihres Benutzers erstellt wurden</span><span class="sxs-lookup"><span data-stu-id="f7dc0-109">Build custom playlists and subcategories crafted specifically for your user's needs</span></span>
- <span data-ttu-id="f7dc0-110">Erstellen sie Angebotsseiten mit Inhalten, die gefiltert wurden, um Geschäftsergebnisse zu unterstützen, z. B. die Einführung von Microsoft Teams, Outlook mobile oder die Zusammenarbeit mit Microsoft 365 zu fördern.</span><span class="sxs-lookup"><span data-stu-id="f7dc0-110">Build landing pages with content filtered to support business outcomes, such as driving the adoption of Microsoft Teams, Outlook mobile, or working more collaboratively with Microsoft 365.</span></span>

![Allgemeine Microsoft-Lernpfade-Fotosammlung.](media/cg-introducing.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="f7dc0-112">Anforderungen und Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="f7dc0-112">Requirements and Permissions</span></span>

<span data-ttu-id="f7dc0-113">Bevor Sie mit den Anleitungen zum Anpassen von Lernpfaden beginnen, stellen Sie sicher, dass Lernpfade von Ihrem SharePoint-Mandantenadministrator eingerichtet wurden.</span><span class="sxs-lookup"><span data-stu-id="f7dc0-113">Before getting started with the Customize learning pathways guidance, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="f7dc0-114">Wenn Sie nicht sicher sind, ob sie eingerichtet wurde, wenden Sie sich an Ihren SharePoint-Mandantenadministrator, um zu überprüfen, ob Lernpfade bereitgestellt wurden.</span><span class="sxs-lookup"><span data-stu-id="f7dc0-114">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="f7dc0-115">Achten Sie außerdem darauf, die URL der SharePoint-Website für Lernpfade zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="f7dc0-115">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="f7dc0-116">Wenn Sie der Mandantenadministrator sind und keine Lernpfade bereitgestellt wurden, finden Sie weitere Informationen unter [Bereitstellen von Lernpfaden](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="f7dc0-116">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="f7dc0-117">Berechtigungen zum Bereitstellen von Lernpfaden</span><span class="sxs-lookup"><span data-stu-id="f7dc0-117">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="f7dc0-118">Mandantenadministrator, auch als globaler Office 365-Administrator bekannt</span><span class="sxs-lookup"><span data-stu-id="f7dc0-118">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="f7dc0-119">Der SharePoint-Websitesammlungsadministrator mit Besitzerberechtigungen für die Website</span><span class="sxs-lookup"><span data-stu-id="f7dc0-119">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="f7dc0-120">Berechtigungen zum Verwenden von Verwaltungsfeatures für Lernpfade</span><span class="sxs-lookup"><span data-stu-id="f7dc0-120">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="f7dc0-121">Websitesammlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="f7dc0-121">Site Collection Administrator</span></span>
- <span data-ttu-id="f7dc0-122">Berechtigungen für SharePoint-Besitzer oder -Mitglieder</span><span class="sxs-lookup"><span data-stu-id="f7dc0-122">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="f7dc0-123">Berechtigungen zur Verwendung der Lernpfadwebsite als Benutzer</span><span class="sxs-lookup"><span data-stu-id="f7dc0-123">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="f7dc0-124">Office 365-Benutzerberechtigungen/Berechtigungen für SharePoint-Websitebesucher oder höher</span><span class="sxs-lookup"><span data-stu-id="f7dc0-124">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="f7dc0-125">Erste Schritte der Anpassung</span><span class="sxs-lookup"><span data-stu-id="f7dc0-125">Get started with customization</span></span>
<span data-ttu-id="f7dc0-126">Nachdem Sie sichergestellt haben, dass Sie über die erforderlichen Berechtigungen zum Anpassen der Website und des Webteils verfügen, ist es an der Zeit, mit dem Anpassungsprozess zu beginnen.</span><span class="sxs-lookup"><span data-stu-id="f7dc0-126">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="f7dc0-127">Informationen zu den ersten Schritte finden [Sie unter Go to the learning pathways site](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="f7dc0-127">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>