---
title: Feilsøke OneDrive-ytelse
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757894"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="646d6-102">Feilsøke OneDrive-ytelse</span><span class="sxs-lookup"><span data-stu-id="646d6-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="646d6-103">Hvis du opplever en tregere enn forventet synkronisering, eller lignende ytelses problemer med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="646d6-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="646d6-104">Bekreft at det ikke er noen kjente problemer med [instrument bordet for tjeneste tilstand](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="646d6-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="646d6-105">[Aktiver filer ved behov](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) , slik at du kan få tilgang til alle filene dine i OneDrive uten å måtte laste ned alle og bruke lagrings plass på enheten.</span><span class="sxs-lookup"><span data-stu-id="646d6-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="646d6-106">[Se gjennom anbefalte Fremgangs måter](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for nettverks planlegging og ytelse.</span><span class="sxs-lookup"><span data-stu-id="646d6-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="646d6-107">[Maksimer opp-og nedlastingshastighet](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), spesielt hvis du synkroniserer en enhet for første gang.</span><span class="sxs-lookup"><span data-stu-id="646d6-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="646d6-108">Hvis du synkroniserer et bibliotek med flere enn 100 000 elementer, kan OneDrive-synkronisering se fast ut i lang tid, eller statusen viser behandlings 0KB av xMB.</span><span class="sxs-lookup"><span data-stu-id="646d6-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="646d6-109">[Lær mer om hvordan du synkroniserer mer enn 100 000 filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) i tillegg til den [støttede grensen på 300 000 filer i OneDrive](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="646d6-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="646d6-110">Når en bruker overskrider bruks begrensninger, begrenser SharePoint Online flere forespørsler fra denne bruker kontoen for en kort periode.</span><span class="sxs-lookup"><span data-stu-id="646d6-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="646d6-111">Alle bruker handlinger begrenses mens begrensningen er i bruk.</span><span class="sxs-lookup"><span data-stu-id="646d6-111">All user actions are throttled while the throttle is in effect.</span></span>
