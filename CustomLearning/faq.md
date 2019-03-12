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
# <a name="frequently-asked-questions"></a><span data-ttu-id="4923c-103">Häufig gestellte Fragen</span><span class="sxs-lookup"><span data-stu-id="4923c-103">Frequently Asked Questions</span></span>

### <a name="1-what-are-the-requirements-for-installing-custom-learning-for-office-365-into-my-tenant-environment"></a><span data-ttu-id="4923c-104">1. Was sind die Anforderungen für die Installation von benutzerdefiniertem Learning für Office 365 in meine Mandanten Umgebung?</span><span class="sxs-lookup"><span data-stu-id="4923c-104">1. What are the requirements for installing Custom Learning for Office 365 into my tenant environment?</span></span>

- <span data-ttu-id="4923c-105">SharePoint Online-und Kommunikationswebsites aktiviert.</span><span class="sxs-lookup"><span data-stu-id="4923c-105">SharePoint Online and Communication Sites enabled.</span></span>
- <span data-ttu-id="4923c-106">Die Person, die CLO365 bereitstellen soll, muss der mandantenadministrator des Zielmandanten für die Installation sein.</span><span class="sxs-lookup"><span data-stu-id="4923c-106">The individual that will be provisioning CLO365 must be the tenant administrator of the target tenant for install.</span></span>
- <span data-ttu-id="4923c-107">Ein Mandanten-App-Katalog muss innerhalb der Option "Apps" im SharePoint Admin Center verfügbar sein.</span><span class="sxs-lookup"><span data-stu-id="4923c-107">A tenant 'App Catalog' must be available within the 'Apps' option of the SharePoint Admin Center.</span></span>
- <span data-ttu-id="4923c-108">Die Person, die CLO365 bereitstellen soll, muss ein Websitesammlungsadministrator des App-Katalogs im Zielmandanten für die Installation sein.</span><span class="sxs-lookup"><span data-stu-id="4923c-108">The individual that will be provisioning CLO365 must be a site collection administrator of the app catalog in the target tenant for install.</span></span>

### <a name="2-what-languages-is-custom-learning-for-office-365-available-in"></a><span data-ttu-id="4923c-109">2. in welchen Sprachen ist benutzerdefiniertes lernen für Office 365 in verfügbar?</span><span class="sxs-lookup"><span data-stu-id="4923c-109">2. What languages is Custom Learning for Office 365 available in?</span></span>

<span data-ttu-id="4923c-110">Benutzerdefiniertes lernen für Office 365 ist derzeit nur in englischer Sprache verfügbar.</span><span class="sxs-lookup"><span data-stu-id="4923c-110">Custom Learning for Office 365 is currently available only in English.</span></span> <span data-ttu-id="4923c-111">Die automatische End-to-End-propositionierung funktioniert nur mit englischen Mandanten.</span><span class="sxs-lookup"><span data-stu-id="4923c-111">Automatic end-to-end provisioning only works with English tenants.</span></span> <span data-ttu-id="4923c-112">In zukünftigen Versionen können zusätzliche Sprachen hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="4923c-112">Additional languages may be added at in future releases.</span></span>

### <a name="3-how-long-will-it-take-to-install-the-site-in-our-tenant-environment"></a><span data-ttu-id="4923c-113">3. wie lange dauert es, bis die Website in unserer Mandanten Umgebung installiert wird?</span><span class="sxs-lookup"><span data-stu-id="4923c-113">3. How long will it take to install the site in our tenant environment?</span></span>

<span data-ttu-id="4923c-114">Basierend auf unseren Tests der Installation sollte es weniger als 15 Minuten dauern.</span><span class="sxs-lookup"><span data-stu-id="4923c-114">Based on our testing of the installation, it should take less than 15 minutes.</span></span> <span data-ttu-id="4923c-115">Dies umfasst nicht die Zeit, die zum Anpassen der Website an Ihre Anforderungen erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="4923c-115">This does not include time required to customize the site to your requirements.</span></span>

### <a name="4-can-we-make-the-custom-learning-for-office-365-a-subsite-of-our-primary-sharepoint-site-collection"></a><span data-ttu-id="4923c-116">4. können wir das benutzerdefinierte Learning für Office 365 zu einer Unterwebsite unserer primären SharePoint-Websitesammlung machen?</span><span class="sxs-lookup"><span data-stu-id="4923c-116">4. Can we make the Custom learning for Office 365 a subsite of our primary SharePoint site collection?</span></span>

<span data-ttu-id="4923c-117">Nein.</span><span class="sxs-lookup"><span data-stu-id="4923c-117">No.</span></span> <span data-ttu-id="4923c-118">Die Website basiert auf einer Kommunikationswebsite Vorlage, die immer als Stammwebsitesammlung gedacht ist.</span><span class="sxs-lookup"><span data-stu-id="4923c-118">The site is based on a communication site template, which is always meant to be a root site collection.</span></span>

> [!NOTE]
> <span data-ttu-id="4923c-119">Es ist wichtig, die Berechtigungen zu berücksichtigen, die Ihre Endbenutzer für den Zugriff auf die Website benötigen.</span><span class="sxs-lookup"><span data-stu-id="4923c-119">It is important to consider the permissions your end users will need to access the site.</span></span> <span data-ttu-id="4923c-120">Die meisten Organisationen haben Sicherheits-oder Benutzergruppen definiert.</span><span class="sxs-lookup"><span data-stu-id="4923c-120">Most organizations have defined security or user groups.</span></span> <span data-ttu-id="4923c-121">Sie müssen dem neuen Schulungsportal die entsprechenden Sicherheitsgruppen hinzufügen, sobald Sie bereit sind, es in Ihrer Mitarbeiter Community zu starten.</span><span class="sxs-lookup"><span data-stu-id="4923c-121">You must add the appropriate security groups to your new training portal once you are ready to launch it to your employee community.</span></span>

### <a name="5-i-need-to-reinstall-the-site-what-should-i-do"></a><span data-ttu-id="4923c-122">5. ich muss die Website neu installieren; Was soll ich tun?</span><span class="sxs-lookup"><span data-stu-id="4923c-122">5. I need to reinstall the site; what should I do?</span></span>

<span data-ttu-id="4923c-123">BeFolgen Sie die [hier](custom_provision.md)veröffentlichten Installationsanweisungen.</span><span class="sxs-lookup"><span data-stu-id="4923c-123">Follow the installation instructions published [here](custom_provision.md).</span></span>

> [!NOTE]
> <span data-ttu-id="4923c-124">Wenn Sie in Ihrer vorherigen Installation die Telemetrie deaktiviert hatten und die Telemetrie deaktiviert bleiben möchten, müssen Sie die Anweisungen zum Deaktivieren der Telemetrie hier befolgen.</span><span class="sxs-lookup"><span data-stu-id="4923c-124">If you had disabled telemetry in your prior installation and would like to continue with telemetry disabled, you will need to follow the instructions for disabling the telemetry here.</span></span>

### <a name="6-we-made-updates-to-our-implementation-of-custom-learning-for-office-365-will-we-lose-these-updates-made-to-site-template-playlists-if-we-reinstall-the-site"></a><span data-ttu-id="4923c-125">6. Wir haben Updates für unsere Implementierung von Custom Learning für Office 365.</span><span class="sxs-lookup"><span data-stu-id="4923c-125">6. We made updates to our implementation of Custom Learning for Office 365.</span></span> <span data-ttu-id="4923c-126">Werden diese Updates (an Websitevorlage, Wiedergabelisten) verloren gehen, wenn wir die Website neu installieren?</span><span class="sxs-lookup"><span data-stu-id="4923c-126">Will we lose these updates (made to site template, playlists) if we reinstall the site?</span></span>

<span data-ttu-id="4923c-127">Anpassungen an einzelnen Seiten und benutzerdefinierten Wiedergabelisten gehen verloren, wenn Sie die Website über Ihre aktuelle Installation neu installieren.</span><span class="sxs-lookup"><span data-stu-id="4923c-127">Customizations to individual pages and custom playlists will be lost if you reinstall the site over your current installation.</span></span>  