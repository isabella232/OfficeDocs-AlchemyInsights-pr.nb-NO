---
title: Feilsøke OneDrive-ytelse
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 197a84c5f69f9e58460925049345263743fe78ee
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43733207"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="ae28e-102">Feilsøke OneDrive-ytelse</span><span class="sxs-lookup"><span data-stu-id="ae28e-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="ae28e-103">Hvis du opplever en langsommere enn forventet synkronisering, eller lignende ytelsesproblemer med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="ae28e-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="ae28e-104">Bekreft at det ikke finnes noen kjente problemer ved hjelp av [instrumentbordet for tjenestetilstand](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="ae28e-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="ae28e-105">[Aktiver filer på forespørsel,](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) slik at du kan få tilgang til alle filene dine i OneDrive uten å måtte laste ned dem alle og bruke lagringsplass på enheten.</span><span class="sxs-lookup"><span data-stu-id="ae28e-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="ae28e-106">[Se gjennom anbefalte fremgangsmåter](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for nettverksplanlegging og ytelse.</span><span class="sxs-lookup"><span data-stu-id="ae28e-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="ae28e-107">[Maksimer opplastings- og nedlastingshastigheten](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), spesielt hvis du synkroniserer en enhet for første gang.</span><span class="sxs-lookup"><span data-stu-id="ae28e-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="ae28e-108">Hvis du synkroniserer et bibliotek med mer enn 100 000 elementer, kan OneDrive-synkronisering virke fast i lang tid, eller statusen viser behandling av 0 kB xMB."</span><span class="sxs-lookup"><span data-stu-id="ae28e-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="ae28e-109">[Finn ut mer om synkronisering av mer enn 100 000 filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) samt [OneDrives støttede grense på 300 000 filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="ae28e-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="ae28e-110">Når en bruker overskrider bruksgrenser, struper SharePoint Online ytterligere forespørsler fra denne brukerkontoen i en kort periode.</span><span class="sxs-lookup"><span data-stu-id="ae28e-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="ae28e-111">Alle brukerhandlinger struper mens gassen er i kraft.</span><span class="sxs-lookup"><span data-stu-id="ae28e-111">All user actions are throttled while the throttle is in effect.</span></span>
