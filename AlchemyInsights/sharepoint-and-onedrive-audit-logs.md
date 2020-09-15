---
title: Klassiske rapporter for overvåkings Logg for SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662217"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="d746b-102">Overvåkings logger for SharePoint og OneDrive</span><span class="sxs-lookup"><span data-stu-id="d746b-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="d746b-103">SharePoint-klassiske overvåkings logger</span><span class="sxs-lookup"><span data-stu-id="d746b-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="d746b-104">SPO eldre overvåking ble overført til Unified Audit log (UAL).</span><span class="sxs-lookup"><span data-stu-id="d746b-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="d746b-105">Alle SPO eldre overvåkings rapporter blir nå slått på via UAL, og de eldre overvåkings signalene har blitt overført til UAL.</span><span class="sxs-lookup"><span data-stu-id="d746b-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="d746b-106">Taste endringer:</span><span class="sxs-lookup"><span data-stu-id="d746b-106">Key changes:</span></span>

* <span data-ttu-id="d746b-107">Trimming er ikke tilgjengelig som en funksjon.</span><span class="sxs-lookup"><span data-stu-id="d746b-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="d746b-108">Det er ikke mulig å velge bestemte hendelser som skal overvåkes.</span><span class="sxs-lookup"><span data-stu-id="d746b-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="d746b-109">Se [dette dokumentet](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for en fullstendig liste over overvåkede hendelser som er tilgjengelige som standard.</span><span class="sxs-lookup"><span data-stu-id="d746b-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="d746b-110">**Plasserings** alternativet under **tilpassede rapporter** er ikke tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="d746b-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="d746b-111">Alternativet for **åpning eller nedlasting av dokument** hendelser er ikke tilgjengelig.</span><span class="sxs-lookup"><span data-stu-id="d746b-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="d746b-112">Konfigurere overvåkings innstillinger for en nettsteds samling</span><span class="sxs-lookup"><span data-stu-id="d746b-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="d746b-113">Overvåkede overvåkings logger for SharePoint og OneDrive fra samsvar</span><span class="sxs-lookup"><span data-stu-id="d746b-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="d746b-114">Aktivere/deaktivere Unified revisjons logging</span><span class="sxs-lookup"><span data-stu-id="d746b-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="d746b-115">Ingen ekstra konfigurasjon kreves i SharePoint eller OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d746b-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="d746b-116">Bruk overvåkings logging søk til å kontrollere aktivitet i filen (e), mappe (r), bruker (e), tillatelser:</span><span class="sxs-lookup"><span data-stu-id="d746b-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="d746b-117">Fil-og side aktiviteter</span><span class="sxs-lookup"><span data-stu-id="d746b-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="d746b-118">Mappe aktiviteter</span><span class="sxs-lookup"><span data-stu-id="d746b-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="d746b-119">Aktiviteter for Delings-og tilgangs forespørsler</span><span class="sxs-lookup"><span data-stu-id="d746b-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="d746b-120">Synkroniserings aktiviteter</span><span class="sxs-lookup"><span data-stu-id="d746b-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="d746b-121">Aktiviteter for nettsteds administrasjon</span><span class="sxs-lookup"><span data-stu-id="d746b-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="d746b-122">Hvis du vil ha mer informasjon om hvordan du henter disse hendelsene, kan du se [søke i overvåkings loggen](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="d746b-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
