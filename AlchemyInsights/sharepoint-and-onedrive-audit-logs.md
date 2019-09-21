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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068032"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="9714d-102">Overvåkingslogger for SharePoint og OneDrive</span><span class="sxs-lookup"><span data-stu-id="9714d-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="9714d-103">**SharePoint og OneDrive moderne Unified overvåkingslogger fra samsvar**</span><span class="sxs-lookup"><span data-stu-id="9714d-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="9714d-104">Slå på/av Unified Audit logging</span><span class="sxs-lookup"><span data-stu-id="9714d-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="9714d-105">Ingen ekstra konfigurasjon kreves i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="9714d-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="9714d-106">Bruk sporing av overvåkingslogging til å kontrollere aktiviteten til filen (e), mappe (r), bruker (e), tillatelser:</span><span class="sxs-lookup"><span data-stu-id="9714d-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="9714d-107">Fil-og side aktiviteter</span><span class="sxs-lookup"><span data-stu-id="9714d-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="9714d-108">Mappe aktiviteter</span><span class="sxs-lookup"><span data-stu-id="9714d-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="9714d-109">Dele og få tilgang til forespørsels aktiviteter</span><span class="sxs-lookup"><span data-stu-id="9714d-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="9714d-110">Synkroniserings aktiviteter</span><span class="sxs-lookup"><span data-stu-id="9714d-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="9714d-111">Aktiviteter for områdeadministrasjon</span><span class="sxs-lookup"><span data-stu-id="9714d-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="9714d-112">Hvis du vil ha mer informasjon om hvordan du henter disse hendelsene, kan du se [søke i overvåkingsloggen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="9714d-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="9714d-113">**Klassiske SharePoint-logger for sporing**</span><span class="sxs-lookup"><span data-stu-id="9714d-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="9714d-114">Vi overførte SPO eldre revisjon til Unified overvåkingsloggen (manuell).</span><span class="sxs-lookup"><span data-stu-id="9714d-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="9714d-115">Dette betyr i hovedsak at alle SPO eldre revisjonsrapporter vil nå bli drevet gjennom manuell, og de eldre revisjons signalene har blitt overført til manuell.</span><span class="sxs-lookup"><span data-stu-id="9714d-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="9714d-116">Viktige endringer:</span><span class="sxs-lookup"><span data-stu-id="9714d-116">Key changes:</span></span>

- <span data-ttu-id="9714d-117">Trimming som en funksjon er ikke tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="9714d-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="9714d-118">Delen der du velger bestemte hendelser som skal overvåkes, er ikke tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="9714d-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="9714d-119">Vennligst referer til [dette dokumentet](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for en fullstendig liste over overvåkede hendelser som er tilgjengelige som standard.</span><span class="sxs-lookup"><span data-stu-id="9714d-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="9714d-120">Alternativet "location" under **tilpassede rapporter** er ikke tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="9714d-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="9714d-121">Hendelser som åpner eller laster ned dokumenter, er ikke tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="9714d-121">“Opening or downloading documents” events is NOT available.</span></span> 

