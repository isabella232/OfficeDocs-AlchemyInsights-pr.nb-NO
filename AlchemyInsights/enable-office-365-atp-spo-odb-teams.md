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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801062"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="76161-102">Aktivere Microsoft Defender for Office 365 for SharePoint Online, OneDrive og Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="76161-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="76161-103">Gå til https://protection.office.com og Logg på.</span><span class="sxs-lookup"><span data-stu-id="76161-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="76161-104">Velg sikre **administrasjons**  >  **policyer** for  >  **klarerte vedlegg** .</span><span class="sxs-lookup"><span data-stu-id="76161-104">Choose **Threat management** > **Policy** > **Safe Attachments** .</span></span>
3. <span data-ttu-id="76161-105">Velg **Aktiver ATP for SharePoint, OneDrive og Microsoft Teams** , og klikk deretter **Lagre** .</span><span class="sxs-lookup"><span data-stu-id="76161-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save** .</span></span>
4. <span data-ttu-id="76161-106">Anbefaler Som global administrator eller administrator for SharePoint Online kjører du cmdleten [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) med **DisallowInfectedFileDownload** -parameteren angitt til *sann* .</span><span class="sxs-lookup"><span data-stu-id="76161-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true* .</span></span>
5. <span data-ttu-id="76161-107">Anbefaler [Konfigurer varsler](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for oppdagede filer.</span><span class="sxs-lookup"><span data-stu-id="76161-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="76161-108">ATP vil skal kunne skanne hver enkelt fil i SharePoint Online, OneDrive eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="76161-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="76161-109">Filer skannes asynkront, gjennom en prosess som bruker hendelser for Delings-og gjeste aktivitet, sammen med smarte heuristikk og trussel signaler for å identifisere skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="76161-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="76161-110">Se [ATP for SharePoint, OneDrive og Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="76161-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>