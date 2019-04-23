---
author: pkrebs
ms.author: pkrebs
title: Übersicht
ms.date: 02/18/2019
description: Übersicht über benutzerdefiniertes lernen für Office 365 für Administratoren
ms.openlocfilehash: 6aee3a93a5109b37e43a7118bd98ca31e8b9ac1f
ms.sourcegitcommit: 775d6807291ab263eea5ec649d9aaf1933fb41ca
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32055635"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="4c8de-103">Anpassen der Lernumgebung</span><span class="sxs-lookup"><span data-stu-id="4c8de-103">Customize the Learning Experience</span></span>

<span data-ttu-id="4c8de-104">Einführung in benutzerdefiniertes lernen für Office 365, eine neue Lösung von Microsoft entwickelt, um die Verwendung und Akzeptanz von Office 365 in einer Organisation zu beschleunigen.</span><span class="sxs-lookup"><span data-stu-id="4c8de-104">Introducing Custom Learning for Office 365, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="4c8de-105">Mit benutzerdefiniertem lernen haben Sie folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="4c8de-105">With Custom Learning, you can:</span></span>
- <span data-ttu-id="4c8de-106">Anpassen von Office 365 Lern-und Adoptions Inhalten für Ihre Umgebung</span><span class="sxs-lookup"><span data-stu-id="4c8de-106">Tailor Office 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="4c8de-107">Ein-oder Ausblenden von Inhalten, um die in Ihrer Organisation unterstützten Dienste oder Features widerzuspiegeln</span><span class="sxs-lookup"><span data-stu-id="4c8de-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="4c8de-108">Halten Sie Ihre Inhalte und Benutzer mit einem aktuellen Feed für das Erlernen von Inhalten von Microsoft auf dem neuesten Stand.</span><span class="sxs-lookup"><span data-stu-id="4c8de-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="4c8de-109">Erstellen von benutzerdefinierten Wiedergabelisten und Kategorien, die speziell für die Anforderungen Ihrer Benutzer erstellt wurden</span><span class="sxs-lookup"><span data-stu-id="4c8de-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![CG-Introducing. png](media/cg-introducing.png)

## <a name="how-does-custom-learning-work"></a><span data-ttu-id="4c8de-111">Wie funktioniert das benutzerdefinierte lernen?</span><span class="sxs-lookup"><span data-stu-id="4c8de-111">How does Custom Learning work?</span></span>

<span data-ttu-id="4c8de-112">Benutzerdefiniertes lernen für Office 365 (benutzerdefiniertes lernen für kurze Zeit) besteht aus drei Teilen:</span><span class="sxs-lookup"><span data-stu-id="4c8de-112">Custom Learning for Office 365 (Custom Learning for short) consists of three parts:</span></span> 
1. <span data-ttu-id="4c8de-113">Live-Feeds von Inhalten aus einem Microsoft Online-Katalog</span><span class="sxs-lookup"><span data-stu-id="4c8de-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="4c8de-114">eine SharePoint-Kommunikationswebsite</span><span class="sxs-lookup"><span data-stu-id="4c8de-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="4c8de-115">ein SharePoint-Webpart</span><span class="sxs-lookup"><span data-stu-id="4c8de-115">a SharePoint web part</span></span> 

![CG-howitworks. png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="4c8de-117">Anforderungen und Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="4c8de-117">Requirements and Permissions</span></span>

<span data-ttu-id="4c8de-118">Bevor Sie mit diesem Handbuch beginnen, sollten Sie sicherstellen, dass benutzerdefiniertes lernen von Ihrem SharePoint-Mandanten Administrator eingerichtet wurde.</span><span class="sxs-lookup"><span data-stu-id="4c8de-118">Before getting started with this guide, ensure that Custom Learning has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="4c8de-119">Wenn Sie nicht sicher sind, ob es eingerichtet wurde, wenden Sie sich an Ihren SharePoint-mandantenadministrator, um zu überprüfen, ob benutzerdefiniertes lernen bereitgestellt wurde.</span><span class="sxs-lookup"><span data-stu-id="4c8de-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that Custom Learning has been provisioned.</span></span> <span data-ttu-id="4c8de-120">Stellen Sie außerdem sicher, dass Sie die URL der benutzerdefinierten Learning SharePoint-Website abrufen.</span><span class="sxs-lookup"><span data-stu-id="4c8de-120">Also be sure to get the URL of the Custom Learning SharePoint site.</span></span> <span data-ttu-id="4c8de-121">Wenn Sie der Mandanten Administrator sind und benutzerdefiniertes lernen nicht eingerichtet wurde, finden Sie weitere Informationen unter Einrichten von [BenutzerdefiniertEm lernen](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="4c8de-121">If you are the Tenant Administrator and Custom Learning has not been provisioned, see [Provision Custom Learning](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-custom-learning"></a><span data-ttu-id="4c8de-122">Berechtigungen zum Einrichten von benutzerdefiniertem lernen</span><span class="sxs-lookup"><span data-stu-id="4c8de-122">Permissions to provision Custom Learning</span></span>

- <span data-ttu-id="4c8de-123">MandantenAdministrator, auch bekannt als globaler Office 365-Administrator</span><span class="sxs-lookup"><span data-stu-id="4c8de-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="4c8de-124">SharePoint-Website Sammlungs Administrator mit Besitzer Berechtigungen für die Website</span><span class="sxs-lookup"><span data-stu-id="4c8de-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-custom-learning-administration-features"></a><span data-ttu-id="4c8de-125">Berechtigungen für die Verwendung von benutzerdefinierten Lern Verwaltungsfeatures</span><span class="sxs-lookup"><span data-stu-id="4c8de-125">Permissions to use Custom Learning Administration features</span></span>

- <span data-ttu-id="4c8de-126">Websitesammlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="4c8de-126">Site Collection Administrator</span></span>
- <span data-ttu-id="4c8de-127">SharePoint-Besitzer-oder Mitgliedsberechtigungen</span><span class="sxs-lookup"><span data-stu-id="4c8de-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-custom-learning-site-as-a-user"></a><span data-ttu-id="4c8de-128">Berechtigungen zum Verwenden der benutzerdefinierten Lernsite als Benutzer</span><span class="sxs-lookup"><span data-stu-id="4c8de-128">Permissions to use the Custom Learning site as a user</span></span>

- <span data-ttu-id="4c8de-129">Office 365-Benutzerberechtigungen/SharePoint-Websitebesucher Berechtigungen oder höher</span><span class="sxs-lookup"><span data-stu-id="4c8de-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="4c8de-130">Erste Schritte mit der Anpassung</span><span class="sxs-lookup"><span data-stu-id="4c8de-130">Get started with customization</span></span>
<span data-ttu-id="4c8de-131">Nachdem Sie sichergestellt haben, dass Sie über die erforderlichen Berechtigungen zum Anpassen der Website und des Webparts verfügen, ist es an der Zeit, mit dem Anpassungsprozess zu beginnen.</span><span class="sxs-lookup"><span data-stu-id="4c8de-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="4c8de-132">Weitere Informationen finden Sie unter [Wechseln zur benutzerdefinierten Lernsite](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="4c8de-132">To get started, see [Go to the Custom Learning Site](custom_goto.md).</span></span>