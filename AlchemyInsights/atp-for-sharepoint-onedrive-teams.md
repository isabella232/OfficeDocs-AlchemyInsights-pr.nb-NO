---
title: ATP for SharePoint-, OneDrive- og Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508421"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="85f59-102">ATP for SharePoint-, OneDrive- og Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="85f59-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="85f59-103">Følg denne fremgangsmåten for å aktivere avansert trusselbeskyttelse:</span><span class="sxs-lookup"><span data-stu-id="85f59-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="85f59-104">Gå til [https://protection.office.com](https://protection.office.com) og logg på med en global administrator- eller sikkerhetsadministratorkonto.</span><span class="sxs-lookup"><span data-stu-id="85f59-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="85f59-105">Velg **Policysikre** vedlegg i den venstre navigasjonsruten under **Trusselbehandling** \> **Safe Attachments**.</span><span class="sxs-lookup"><span data-stu-id="85f59-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="85f59-106">Velg **Aktiver ATP for SharePoint, OneDrive og Microsoft Teams**.</span><span class="sxs-lookup"><span data-stu-id="85f59-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="85f59-107">[Opprett en policy for aktivitetsvarsler](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) for å motta varsler når vi oppdager skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="85f59-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="85f59-108">Hvis du vil ha fullstendige instruksjoner, kan du se dette [emnet](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="85f59-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="85f59-109">**Merk:** Etter utforming skanner ikke ATP hver enkelt fil i SharePoint Online, OneDrive for Business eller Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="85f59-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="85f59-110">Filer skannes asynkront av en prosess som bruker delingsaktivitet, gjesteaktivitet og trusselsignaler til å identifisere skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="85f59-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="85f59-111">Hvis du vil ha mer informasjon, kan du se dette [emnet](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="85f59-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
