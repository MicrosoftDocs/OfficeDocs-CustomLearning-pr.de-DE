---
author: pkrebs
ms.author: pkrebs
title: Übersicht
ms.date: 02/18/2019
description: Übersicht über Microsoft 365 Lern Pfade
ms.openlocfilehash: 74fac090177ad8009155e21a977b05ee2b742b3b
ms.sourcegitcommit: f5a7079d56598c14aef2f4b886c025a59ba89276
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/21/2019
ms.locfileid: "34247848"
---
# <a name="customize-the-learning-experience"></a><span data-ttu-id="983c8-103">Anpassen der Lernerfahrung</span><span class="sxs-lookup"><span data-stu-id="983c8-103">Customize the learning experience</span></span>

<span data-ttu-id="983c8-104">Einführung in Microsoft 365-Lern Pfade, eine neue Lösung von Microsoft, die die Verwendung und Übernahme von Office 365 in einer Organisation beschleunigen soll.</span><span class="sxs-lookup"><span data-stu-id="983c8-104">Introducing Microsoft 365 learning pathways, a new solution from Microsoft designed to speed the usage and adoption of Office 365 within an organization.</span></span> <span data-ttu-id="983c8-105">Mit Learning pathwyas können Sie Folgendes tun:</span><span class="sxs-lookup"><span data-stu-id="983c8-105">With learning pathwyas, you can:</span></span>
- <span data-ttu-id="983c8-106">Anpassen von Microsoft 365 Lern-und Adoptions Inhalten für Ihre Umgebung</span><span class="sxs-lookup"><span data-stu-id="983c8-106">Tailor Microsoft 365 learning and adoption content for your environment</span></span> 
- <span data-ttu-id="983c8-107">Ausblenden oder Anzeigen von Inhalten, um die in Ihrer Organisation unterstützten Dienste oder Features widerzuspiegeln</span><span class="sxs-lookup"><span data-stu-id="983c8-107">Hide or show content to reflect the services or features supported in your organization</span></span> 
- <span data-ttu-id="983c8-108">Halten Sie Ihre Inhalte und Benutzer mit einem aktuellen Feed für Lerninhalte von Microsoft auf dem neuesten Stand.</span><span class="sxs-lookup"><span data-stu-id="983c8-108">Keep your content and users current with an up-to-date feed of learning content from Microsoft</span></span> 
- <span data-ttu-id="983c8-109">Erstellen benutzerdefinierter Wiedergabelisten und Kategorien, die speziell für die Anforderungen Ihrer Benutzer erstellt wurden</span><span class="sxs-lookup"><span data-stu-id="983c8-109">Build custom playlists and categories crafted specifically for your user's needs</span></span>

![CG-Introducing. png](media/cg-introducing.png)

## <a name="how-does-learning-pathways-work"></a><span data-ttu-id="983c8-111">Wie funktionieren Lern Pfade?</span><span class="sxs-lookup"><span data-stu-id="983c8-111">How does learning pathways work?</span></span>

<span data-ttu-id="983c8-112">Lern Pfade für Office 365 (kurz Lernpfade) bestehen aus drei Teilen:</span><span class="sxs-lookup"><span data-stu-id="983c8-112">learning pathways for Office 365 (learning pathways for short) consists of three parts:</span></span> 
1. <span data-ttu-id="983c8-113">ein Live-Feed von Inhalten aus einem Microsoft Online-Katalog</span><span class="sxs-lookup"><span data-stu-id="983c8-113">a live feed of content from a Microsoft online catalog</span></span>
2. <span data-ttu-id="983c8-114">eine SharePoint-Kommunikationswebsite</span><span class="sxs-lookup"><span data-stu-id="983c8-114">a SharePoint communication site</span></span>
3. <span data-ttu-id="983c8-115">eines SharePoint-Webparts</span><span class="sxs-lookup"><span data-stu-id="983c8-115">a SharePoint web part</span></span> 

![CG-howitworks. png](media/cg-howitworks.png)

## <a name="requirements-and-permissions"></a><span data-ttu-id="983c8-117">Anforderungen und Berechtigungen</span><span class="sxs-lookup"><span data-stu-id="983c8-117">Requirements and Permissions</span></span>

<span data-ttu-id="983c8-118">Stellen Sie vor dem ersten Einstieg in dieses Handbuch sicher, dass von Ihrem SharePoint-Mandanten Administrator Lern Pfade eingerichtet wurden.</span><span class="sxs-lookup"><span data-stu-id="983c8-118">Before getting started with this guide, ensure that learning pathways has been set up by your SharePoint Tenant Administrator.</span></span> <span data-ttu-id="983c8-119">Wenn Sie sich nicht sicher sind, ob Sie eingerichtet wurde, wenden Sie sich an Ihren SharePoint-mandantenadministrator, um zu überprüfen, ob Lern Pfade bereitgestellt wurden.</span><span class="sxs-lookup"><span data-stu-id="983c8-119">If you’re not sure if it's been set up, contact your SharePoint tenant administrator to verify that learning pathways has been provisioned.</span></span> <span data-ttu-id="983c8-120">Stellen Sie außerdem sicher, dass Sie die URL der SharePoint-Website für Lern Pfade abrufen.</span><span class="sxs-lookup"><span data-stu-id="983c8-120">Also be sure to get the URL of the learning pathways SharePoint site.</span></span> <span data-ttu-id="983c8-121">Wenn Sie der Mandanten Administrator sind und keine Lern Pfade eingerichtet wurden, finden Sie weitere Informationen unter [Bereitstellungspfade](custom_provision.md).</span><span class="sxs-lookup"><span data-stu-id="983c8-121">If you are the Tenant Administrator and learning pathways has not been provisioned, see [Provision learning pathways](custom_provision.md).</span></span> 

### <a name="permissions-to-provision-learning-pathways"></a><span data-ttu-id="983c8-122">Berechtigungen zur Vermittlung von Lernpfaden</span><span class="sxs-lookup"><span data-stu-id="983c8-122">Permissions to provision learning pathways</span></span>

- <span data-ttu-id="983c8-123">Mandantenadministrator, auch bekannt als Office 365 globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="983c8-123">Tenant Administrator, also known as Office 365 Global Administrator</span></span>
- <span data-ttu-id="983c8-124">SharePoint-Website Sammlungs Administrator mit Besitzer Berechtigungen für die Website</span><span class="sxs-lookup"><span data-stu-id="983c8-124">SharePoint Site Collection Administrator with Owner permissions on the site</span></span>

### <a name="permissions-to-use-learning-pathways-administration-features"></a><span data-ttu-id="983c8-125">Berechtigungen zum Verwenden von Verwaltungsfeatures für Lern Pfade</span><span class="sxs-lookup"><span data-stu-id="983c8-125">Permissions to use learning pathways Administration features</span></span>

- <span data-ttu-id="983c8-126">Websitesammlungsadministrator</span><span class="sxs-lookup"><span data-stu-id="983c8-126">Site Collection Administrator</span></span>
- <span data-ttu-id="983c8-127">SharePoint-Besitzer-oder Mitgliedsberechtigungen</span><span class="sxs-lookup"><span data-stu-id="983c8-127">SharePoint Owner or Member permissions</span></span>

### <a name="permissions-to-use-the-learning-pathways-site-as-a-user"></a><span data-ttu-id="983c8-128">Berechtigungen zum Verwenden der Website für Lern Pfade als Benutzer</span><span class="sxs-lookup"><span data-stu-id="983c8-128">Permissions to use the learning pathways site as a user</span></span>

- <span data-ttu-id="983c8-129">Office 365 Berechtigungen für Benutzer/SharePoint-Websitebesucher oder höher</span><span class="sxs-lookup"><span data-stu-id="983c8-129">Office 365 user permissions/SharePoint Site Visitor permissions or higher</span></span>

## <a name="get-started-with-customization"></a><span data-ttu-id="983c8-130">Erste Schritte bei der Anpassung</span><span class="sxs-lookup"><span data-stu-id="983c8-130">Get started with customization</span></span>
<span data-ttu-id="983c8-131">Nachdem Sie sichergestellt haben, dass Sie über die erforderlichen Berechtigungen zum Anpassen der Website und des Webparts verfügen, ist es an der Zeit, mit dem Anpassungsprozess begonnen zu werden.</span><span class="sxs-lookup"><span data-stu-id="983c8-131">Once you've ensured you have the necessary permissions to customize the site and web part, it's time to get started with the customization process.</span></span> 

- <span data-ttu-id="983c8-132">Informationen zu den ersten Schritten finden Sie unter [Wechseln zur Website für Lern Pfade](custom_goto.md).</span><span class="sxs-lookup"><span data-stu-id="983c8-132">To get started, see [Go to the learning pathways site](custom_goto.md).</span></span>