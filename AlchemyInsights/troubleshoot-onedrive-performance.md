---
title: Feilsøke OneDrive-ytelse
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 222f818c3fd78a19b9952d4703755498bc080910
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822207"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="c1c24-102">Feilsøke OneDrive-ytelse</span><span class="sxs-lookup"><span data-stu-id="c1c24-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="c1c24-103">Hvis du har en tregere enn forventet synkronisering, eller lignende ytelsesproblemer med OneDrive:</span><span class="sxs-lookup"><span data-stu-id="c1c24-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="c1c24-104">Bekreft at det ikke er noen kjente problemer ved bruk av [service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="c1c24-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="c1c24-105">[Aktiver filer på forespørsel](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) slik at du får tilgang til alle filene dine i OneDrive uten å måtte laste ned alle og bruke lagringsplass på enheten.</span><span class="sxs-lookup"><span data-stu-id="c1c24-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="c1c24-106">[Gå gjennom gode fremgangsmåter](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for nettverksplanlegging og-ytelse.</span><span class="sxs-lookup"><span data-stu-id="c1c24-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="c1c24-107">[Maksimer opplastings-og nedlastingshastighet](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), spesielt hvis du synkroniserer en enhet for første gang.</span><span class="sxs-lookup"><span data-stu-id="c1c24-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="c1c24-108">Hvis du synkroniserer et bibliotek med mer enn 100 000 elementer, kan OneDrive-synkronisering virke fast i lang tid, eller statusen viser Processing 0KB av xMB. "</span><span class="sxs-lookup"><span data-stu-id="c1c24-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="c1c24-109">[Finn ut mer om synkronisering av mer enn 100 000 filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) i tillegg [til OneDrive ' s støttede grense på 300 000 filer](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="c1c24-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="c1c24-110">Når en bruker overskrider bruks grensene, throttles SharePoint Online eventuelle ytterligere forespørsler fra denne brukerkontoen i en kort periode.</span><span class="sxs-lookup"><span data-stu-id="c1c24-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="c1c24-111">Alle brukerhandlinger er begrenset når gassen er aktivert.</span><span class="sxs-lookup"><span data-stu-id="c1c24-111">All user actions are throttled while the throttle is in effect.</span></span>
