---
title: Aktivere Atp for Office 365 for SharePoint, OneDrive og Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703435"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="4d291-102">Aktivere avansert trusselbeskyttelse for Office 365 for SharePoint Online, OneDrive og Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="4d291-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="4d291-103">Gå https://protection.office.com til og logg på.</span><span class="sxs-lookup"><span data-stu-id="4d291-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="4d291-104">Velg Policy for **Threat management** > **trusselstyring** > **sikre vedlegg**.</span><span class="sxs-lookup"><span data-stu-id="4d291-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="4d291-105">Velg **Aktiver ATP for SharePoint, OneDrive og Microsoft Teams**, og klikk deretter **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="4d291-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="4d291-106">(Anbefales) Som global administrator eller SharePoint Online-administrator kjører du cmdleten [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med parameteren **DisallowInfectedFileDownload** satt til *true*.</span><span class="sxs-lookup"><span data-stu-id="4d291-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="4d291-107">(Anbefales) [Konfigurer varsler](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for oppdagede filer.</span><span class="sxs-lookup"><span data-stu-id="4d291-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="4d291-108">ATP vil ikke skanne hver enkelt fil i SharePoint Online, OneDrive eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4d291-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="4d291-109">Filer skannes asynkront, gjennom en prosess som bruker deling og gjesteaktivitetshendelser, sammen med smarte heuristikk og trusselsignaler for å identifisere skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="4d291-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="4d291-110">Se [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="4d291-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>