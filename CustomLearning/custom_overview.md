---
author: pkrebs
ms.author: pkrebs
title: Übersicht
ms.date: 02/18/2019
description: Übersicht über benutzerdefiniertes lernen für Office 365 für Administratoren
ms.openlocfilehash: 98187038b66252523c74d88dd9bfd0f217591bc5
ms.sourcegitcommit: e10085e60ca3f38029fde229fb093e6bc4a34203
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/25/2019
ms.locfileid: "30087534"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="8314d-103">Anpassen der Lernumgebung</span><span class="sxs-lookup"><span data-stu-id="8314d-103">Customize the Learning Experience</span></span>

<span data-ttu-id="8314d-p101">Einführung in benutzerdefiniertes lernen für Office 365, eine neue Lösung von Microsoft entwickelt, um die Verwendung und Akzeptanz von Office 365 in einer Organisation zu beschleunigen. Mit benutzerdefiniertem lernen haben Sie folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="8314d-p101">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization. With Custom Learning, you can:</span></span>
- <span data-ttu-id="8314d-106">Anpassen von Office 365 Lern-und Adoptions Inhalten für Ihre Umgebung</span><span class="sxs-lookup"><span data-stu-id="8314d-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="8314d-107">Ein-oder Ausblenden von Inhalten, um die in Ihrer Organisation unterstützten Dienste oder Features widerzuspiegeln</span><span class="sxs-lookup"><span data-stu-id="8314d-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="8314d-108">Halten Sie Ihre Inhalte und Benutzer mit einem aktuellen Feed für das Erlernen von Inhalten von Microsoft auf dem neuesten Stand.</span><span class="sxs-lookup"><span data-stu-id="8314d-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="8314d-109">Erstellen von benutzerdefinierten Wiedergabelisten und Kategorien, die speziell für die Anforderungen Ihrer Benutzer erstellt wurden</span><span class="sxs-lookup"><span data-stu-id="8314d-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![CG-Introducing. png](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="8314d-111">Wie funktioniert das benutzerdefinierte lernen?</span><span class="sxs-lookup"><span data-stu-id="8314d-111">How does Custom Learning work?</span></span>

<span data-ttu-id="8314d-112">Benutzerdefiniertes lernen für Office 365 (benutzerdefiniertes lernen für kurze Zeit) besteht aus drei Teilen:</span><span class="sxs-lookup"><span data-stu-id="8314d-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="8314d-113">Live-Feeds von Inhalten aus einem Microsoft Online-Katalog</span><span class="sxs-lookup"><span data-stu-id="8314d-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="8314d-114">eine SharePoint-Kommunikationswebsite</span><span class="sxs-lookup"><span data-stu-id="8314d-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="8314d-115">ein SharePoint-Webpart</span><span class="sxs-lookup"><span data-stu-id="8314d-115">a SharePoint web part</span></span> 

![CG-howitworks. png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="8314d-117">Anforderungen und Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8314d-117">Requirements and Permissions</span></span>

<span data-ttu-id="8314d-p102">Bevor Sie mit diesem Handbuch beginnen, sollten Sie sicherstellen, dass benutzerdefiniertes lernen von Ihrem SharePoint-mandantenadministrator eingerichtet wurde. Wenn Sie nicht sicher sind, ob es eingerichtet wurde, wenden Sie sich an Ihren SharePoint-mandantenadministrator, um zu überprüfen, ob benutzerdefiniertes lernen installiert wurde. Stellen Sie außerdem sicher, dass Sie die URL der benutzerdefinierten Learning SharePoint-Website abrufen. Wenn Sie der Mandanten Administrator sind und benutzerdefiniertes lernen nicht installiert wurde, finden Sie weitere Informationen unter Custom Learning for Office 365 Installation Guide.</span><span class="sxs-lookup"><span data-stu-id="8314d-p102">Before getting started with this guide, ensure that Custom Learning has been set up by your  SharePoint tenant administrator. If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been installed. Also be sure to get the URL of the Custom Learning SharePoint site. If you are the Tenant Administrator and Custom Learning has not been installed, see the Custom Learning for Office 365 Installation Guide.</span></span> 

### <a name="permissions-to-install-custom-learning"></a><span data-ttu-id="8314d-122">Berechtigungen zum Installieren von benutzerdefiniertem lernen</span><span class="sxs-lookup"><span data-stu-id="8314d-122">Permissions to install Custom Learning</span></span>

- <span data-ttu-id="8314d-123">Office 365 globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="8314d-123">Office 365 Global Administrator</span></span>
- <span data-ttu-id="8314d-124">SharePoint-Administrator</span><span class="sxs-lookup"><span data-stu-id="8314d-124">SharePoint Administrator</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="8314d-125">Berechtigungen für die Verwendung von benutzerdefinierten Lern Verwaltungsfeatures</span><span class="sxs-lookup"><span data-stu-id="8314d-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="8314d-126">Office 365 SharePoint-Administrator/SharePoint-Websitebesitzer Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="8314d-126">Office 365 SharePoint Administrator/SharePoint Site Owner Permissions</span></span>
- <span data-ttu-id="8314d-127">Berechtigungen für SharePoint-Website Sammlungs Administrator/SharePoint-Websitebesitzer</span><span class="sxs-lookup"><span data-stu-id="8314d-127">SharePoint Site Collection Administrator/SharePoint Site Owner Permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="8314d-128">Berechtigungen zum Verwenden der benutzerdefinierten Lernsite als Benutzer</span><span class="sxs-lookup"><span data-stu-id="8314d-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="8314d-129">Office 365-Benutzerberechtigungen/SharePoint-Websitebesucher Berechtigungen oder höher</span><span class="sxs-lookup"><span data-stu-id="8314d-129">Office 365 user permissions/SharePoint Site Visitor Permissions or higher</span></span>


