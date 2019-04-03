---
title: Aktivere Office 365 ATP for SharePoint, OneDrive og Microsoft Team
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031038"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="844a3-102">Aktivere Office 365 Avansert trussel beskyttelse for SharePoint Online, OneDrive og Microsoft Team</span><span class="sxs-lookup"><span data-stu-id="844a3-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="844a3-103">Gå til https://protection.office.com og logger deg på.</span><span class="sxs-lookup"><span data-stu-id="844a3-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="844a3-104">Velg **Threat management** > **Policy** > **Sikker vedlegg**.</span><span class="sxs-lookup"><span data-stu-id="844a3-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="844a3-105">Velg **Slå på ATP-Antallet for SharePoint, OneDrive, og Microsoft Team**, og klikk deretter **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="844a3-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="844a3-106">(Anbefales) Som en global administrator eller en administrator for SharePoint Online, kjører du cmdleten [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med **DisallowInfectedFileDownload** -parameteren angitt til *Sann*.</span><span class="sxs-lookup"><span data-stu-id="844a3-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="844a3-107">(Anbefales) [Angi varsler](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for oppdagede filer.</span><span class="sxs-lookup"><span data-stu-id="844a3-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="844a3-108">ATP vil nFor skanning hver enkelt fil i SharePoint Online, OneDrive, eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="844a3-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="844a3-109">Filer skannes asynkront, gjennom en prosess som bruker deling og gjest aktivitet hendelser, sammen med smart heuristisk og trusselen signaler til å identifisere ondsinnede filer.</span><span class="sxs-lookup"><span data-stu-id="844a3-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="844a3-110">Se [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="844a3-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>