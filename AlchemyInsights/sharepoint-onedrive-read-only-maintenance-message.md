---
title: Skrivebeskyttet for vedlikehold melding når du prøver å bruke SharePoint- eller OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: cc232fba6f502e2b6f282a8c1a1e29221e36b70d
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840524"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="eee58-102">Skrivebeskyttet for vedlikehold melding når du prøver å bruke SharePoint- eller OneDrive</span><span class="sxs-lookup"><span data-stu-id="eee58-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="eee58-103">Brukere kan få en **Skrivebeskyttet for vedlikehold** melding når du prøver å bruke SharePoint- eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="eee58-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive.</span></span>  <span data-ttu-id="eee58-104">I så fall må du kontrollere om det er aktivt vedlikehold oppstår på din leier ved å navigere til [Meldingssentral](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="eee58-104">If so, check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span> <span data-ttu-id="eee58-105">Kontroller også at å kontrollere [Service helse](https://portal.office.com/adminportal/home#/servicehealth) -dashbordet til å se etter veiledningene/hendelser som kan oppstå.</span><span class="sxs-lookup"><span data-stu-id="eee58-105">Also, make sure to check the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) dashboard to check for any advisories/incidents that may be occurring.</span></span>

<span data-ttu-id="eee58-106">Hvis verken Meldingssentral eller tjenesten helse dashboard har lagt merke til noe om gjeldende vedlikehold for din leier, kan dette være en Web-leser bufre problemet.</span><span class="sxs-lookup"><span data-stu-id="eee58-106">If neither the Message Center or Service Health dashboard have noted anything about current maintenance for your tenant, this may be a browser caching issue.</span></span>

<span data-ttu-id="eee58-107">Prøv å tømme hurtigbufferen for webleseren før du navigere til området.</span><span class="sxs-lookup"><span data-stu-id="eee58-107">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="eee58-108">I webleseren Microsoft Edge, velg **Innstillinger**, og velg deretter **Personvern og sikkerhet**.</span><span class="sxs-lookup"><span data-stu-id="eee58-108">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="eee58-109">**Fjern Bla gjennom**, velg **Velg hva du vil fjerne**.</span><span class="sxs-lookup"><span data-stu-id="eee58-109">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="eee58-110">Velg **informasjonskapsler og webområdet for lagrede data**, og velg **Fjern**.</span><span class="sxs-lookup"><span data-stu-id="eee58-110">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="eee58-111">Disse trinnene kan variere når du bruker andre lesere, for eksempel Mozilla Firefox eller Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="eee58-111">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="eee58-112">Et annet alternativ er å åpne SharePoint-området eller OneDrive i et nytt InPrivate-vindu.</span><span class="sxs-lookup"><span data-stu-id="eee58-112">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>