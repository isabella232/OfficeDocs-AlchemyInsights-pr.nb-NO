---
title: Aktivere Office 365 ATP for SharePoint, OneDrive og Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543937"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="1e1c7-102">Aktivere Microsoft Defender for Office 365 for SharePoint Online, OneDrive og Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="1e1c7-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="1e1c7-103">Gå til https://protection.office.com og logg på.</span><span class="sxs-lookup"><span data-stu-id="1e1c7-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="1e1c7-104">Velg **Klarerte vedlegg for** policy for  >    >  **trusselbehandling**.</span><span class="sxs-lookup"><span data-stu-id="1e1c7-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="1e1c7-105">Velg **Aktiver Defender for Office 365 for SharePoint, OneDrive og Microsoft Teams**, og klikk deretter **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="1e1c7-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="1e1c7-106">(Anbefales) Som global administrator eller SharePoint Online-administrator kjører du [Set-SPOTenant-cmdleten](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med **parameteren DisallowInfectedFileDownload** satt til *sann*.</span><span class="sxs-lookup"><span data-stu-id="1e1c7-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="1e1c7-107">(Anbefales) [Konfigurere varsler](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for oppdagede filer.</span><span class="sxs-lookup"><span data-stu-id="1e1c7-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="1e1c7-108">Microsoft Defender for Office 365 vil ikke skanne hver enkelt fil i SharePoint Online, OneDrive eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="1e1c7-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="1e1c7-109">Filer skannes asynkront gjennom en prosess som bruker delings- og gjesteaktivitetshendelser, sammen med smart heuristikk og trusselsignaler for å identifisere skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="1e1c7-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="1e1c7-110">Se [Microsoft Defender for Office 365 for SharePoint, OneDrive og Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="1e1c7-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>