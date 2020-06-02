---
title: Rapporter for klassisk SharePoint-overvåkingslogg
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 0aedb549f11db54d3cd480671fb0767c60680ad3
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509609"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="931dd-102">Overvåkingslogger for SharePoint og OneDrive</span><span class="sxs-lookup"><span data-stu-id="931dd-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="931dd-103">SharePoint klassiske overvåkingslogger</span><span class="sxs-lookup"><span data-stu-id="931dd-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="931dd-104">SPO eldre revisjon ble overført til Unified Audit Log (UAL).</span><span class="sxs-lookup"><span data-stu-id="931dd-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="931dd-105">Alle SPO eldre revisjonsrapporter vil nå bli drevet gjennom UAL, og de eldre revisjonssignalene er overført til UAL.</span><span class="sxs-lookup"><span data-stu-id="931dd-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="931dd-106">Viktige endringer:</span><span class="sxs-lookup"><span data-stu-id="931dd-106">Key changes:</span></span>

* <span data-ttu-id="931dd-107">Trimming er IKKE tilgjengelig som en evne.</span><span class="sxs-lookup"><span data-stu-id="931dd-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="931dd-108">Å velge bestemte hendelser som skal revideres er IKKE tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="931dd-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="931dd-109">Se [dette dokumentet](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for en fullstendig liste over overvåkede hendelser som er tilgjengelige som standard.</span><span class="sxs-lookup"><span data-stu-id="931dd-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="931dd-110">Alternativet **Plassering** under **Tilpassede rapporter** er IKKE tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="931dd-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="931dd-111">Alternativet **Åpne eller laste ned dokumenter** hendelser er IKKE tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="931dd-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="931dd-112">Konfigurere overvåkingsinnstillinger for en områdesamling</span><span class="sxs-lookup"><span data-stu-id="931dd-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="931dd-113">SharePoint og OneDrive moderne enhetlig overvåkingslogger fra samsvar</span><span class="sxs-lookup"><span data-stu-id="931dd-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="931dd-114">Aktivere/deaktivere logging av enhetlig revisjon</span><span class="sxs-lookup"><span data-stu-id="931dd-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="931dd-115">Ingen ekstra konfigurasjon er nødvendig i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="931dd-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="931dd-116">Bruk søk etter overvåkingslogging til å kontrollere aktiviteten til filen(e), mappe(er), bruker(er), tillatelser:</span><span class="sxs-lookup"><span data-stu-id="931dd-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="931dd-117">Fil- og sideaktiviteter</span><span class="sxs-lookup"><span data-stu-id="931dd-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="931dd-118">Mappeaktiviteter</span><span class="sxs-lookup"><span data-stu-id="931dd-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="931dd-119">Delings- og tilgangsforespørselsaktiviteter</span><span class="sxs-lookup"><span data-stu-id="931dd-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="931dd-120">Synkroniseringsaktiviteter</span><span class="sxs-lookup"><span data-stu-id="931dd-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="931dd-121">Aktiviteter for administrasjon av nettsteder</span><span class="sxs-lookup"><span data-stu-id="931dd-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="931dd-122">Hvis du vil ha mer informasjon om hvordan du henter disse hendelsene, kan du se [Søke i overvåkingsloggen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="931dd-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
