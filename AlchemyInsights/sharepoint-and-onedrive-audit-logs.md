---
title: Klassiske overvåkingslogg rapporter for SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992627"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="c69fe-102">Overvåkingslogger for SharePoint og OneDrive</span><span class="sxs-lookup"><span data-stu-id="c69fe-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="c69fe-103">Klassiske SharePoint-logger for sporing</span><span class="sxs-lookup"><span data-stu-id="c69fe-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="c69fe-104">SPO Legacy-overvåking ble overført til Unified overvåkingsloggen (manuell).</span><span class="sxs-lookup"><span data-stu-id="c69fe-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="c69fe-105">Alle alle SPO eldre revisjonsrapporter vil nå bli drevet gjennom manuell, og de eldre revisjons signalene er overført til manuell.</span><span class="sxs-lookup"><span data-stu-id="c69fe-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="c69fe-106">Viktige endringer:</span><span class="sxs-lookup"><span data-stu-id="c69fe-106">Key changes:</span></span>

* <span data-ttu-id="c69fe-107">Trimming er ikke tilgjengelig som en funksjon.</span><span class="sxs-lookup"><span data-stu-id="c69fe-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="c69fe-108">Det er ikke mulig å velge bestemte hendelser som skal overvåkes.</span><span class="sxs-lookup"><span data-stu-id="c69fe-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="c69fe-109">Se [dette dokumentet](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for en fullstendig liste over overvåkede hendelser som er tilgjengelige som standard.</span><span class="sxs-lookup"><span data-stu-id="c69fe-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="c69fe-110">Alternativet **plassering** under **tilpassede rapporter** er ikke tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="c69fe-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="c69fe-111">Alternativet for **åpning eller nedlasting av dokumenter** hendelser er ikke tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="c69fe-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="c69fe-112">Konfigurere overvåkingsinnstillinger for en områdesamling</span><span class="sxs-lookup"><span data-stu-id="c69fe-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="c69fe-113">SharePoint og OneDrive moderne Unified overvåkingslogger fra samsvar</span><span class="sxs-lookup"><span data-stu-id="c69fe-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="c69fe-114">Slå på/av Unified Audit logging</span><span class="sxs-lookup"><span data-stu-id="c69fe-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="c69fe-115">Ingen ekstra konfigurasjon kreves i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="c69fe-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="c69fe-116">Bruk sporing av overvåkingslogging til å kontrollere aktiviteten til filen (e), mappe (r), bruker (e), tillatelser:</span><span class="sxs-lookup"><span data-stu-id="c69fe-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="c69fe-117">Fil-og side aktiviteter</span><span class="sxs-lookup"><span data-stu-id="c69fe-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="c69fe-118">Mappe aktiviteter</span><span class="sxs-lookup"><span data-stu-id="c69fe-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="c69fe-119">Dele og få tilgang til forespørsels aktiviteter</span><span class="sxs-lookup"><span data-stu-id="c69fe-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="c69fe-120">Synkroniserings aktiviteter</span><span class="sxs-lookup"><span data-stu-id="c69fe-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="c69fe-121">Aktiviteter for områdeadministrasjon</span><span class="sxs-lookup"><span data-stu-id="c69fe-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="c69fe-122">Hvis du vil ha mer informasjon om hvordan du henter disse hendelsene, kan du se [søke i overvåkingsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="c69fe-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
