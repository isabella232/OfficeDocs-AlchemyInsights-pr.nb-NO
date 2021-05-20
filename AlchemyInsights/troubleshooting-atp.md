---
title: Feilsøke Microsoft Defender for Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545277"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="2a02b-102">Feilsøke Microsoft Defender for Office 365</span><span class="sxs-lookup"><span data-stu-id="2a02b-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="2a02b-103">**Legger du merke til forsinkelser i meldingsleveringen?**</span><span class="sxs-lookup"><span data-stu-id="2a02b-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="2a02b-104">Bruk alternativet [Dynamisk levering i](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) Microsoft Defender for å Office 365 klarerte vedlegg.</span><span class="sxs-lookup"><span data-stu-id="2a02b-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="2a02b-105">Dette vil bidra til å unngå meldingsforsinkelser samtidig som mottakerne beskyttes mot skadelige filer.</span><span class="sxs-lookup"><span data-stu-id="2a02b-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="2a02b-106">**Vil du rapportere falske positiver eller falske negativer til Microsoft?**</span><span class="sxs-lookup"><span data-stu-id="2a02b-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="2a02b-107">Bruk [Innsendingsutforsker](https://protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="2a02b-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="2a02b-108">-\*\* Visste du at du kan aktivere beskyttelse av klarerte koblinger for intern e-post som sendes mellom mottakere i organisasjonen?\*\* Følg disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="2a02b-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="2a02b-109">Gå til [https://protection.office.com](https://protection.office.com) og logg på med en global administrator- eller sikkerhetsadministratorkonto.</span><span class="sxs-lookup"><span data-stu-id="2a02b-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="2a02b-110">Velg Klarerte koblinger for policy **i** den venstre navigasjonsruten under **Trusselbehandling** \> .</span><span class="sxs-lookup"><span data-stu-id="2a02b-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="2a02b-111">Velg **policyen under Policyer som gjelder** for hele organisasjonen, og klikk **Rediger**.</span><span class="sxs-lookup"><span data-stu-id="2a02b-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="2a02b-112">Under **Innstillinger** aktiverer du **Bruk klarerte koblinger på meldinger som sendes i organisasjonen**.</span><span class="sxs-lookup"><span data-stu-id="2a02b-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
