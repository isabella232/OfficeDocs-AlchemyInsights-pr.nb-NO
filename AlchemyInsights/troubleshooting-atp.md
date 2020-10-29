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
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801452"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="28190-102">Feilsøke Microsoft Defender for Office 365</span><span class="sxs-lookup"><span data-stu-id="28190-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="28190-103">Oppdager du forsinkelser i meldings levering?</span><span class="sxs-lookup"><span data-stu-id="28190-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="28190-104">Bruk alternativet [dynamisk levering](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) i policyen ATP-sikre vedlegg.</span><span class="sxs-lookup"><span data-stu-id="28190-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="28190-105">Dette vil bidra til å unngå meldings forsinkelser under beskyttelse av mottakere fra ondsinnede filer.</span><span class="sxs-lookup"><span data-stu-id="28190-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="28190-106">Vil du rapportere falske positiver eller falske negativer til Microsoft?</span><span class="sxs-lookup"><span data-stu-id="28190-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="28190-107">Bruk denne [koblingen](https://www.microsoft.com/wdsi/filesubmission/) til å sende filer for analyse.</span><span class="sxs-lookup"><span data-stu-id="28190-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="28190-108">Visste du at du kan aktivere beskyttelse mot sikre koblinger for intern e-post som sendes mellom mottakere i organisasjonen?</span><span class="sxs-lookup"><span data-stu-id="28190-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="28190-109">Følg disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="28190-109">Follow these steps:</span></span>

  1. <span data-ttu-id="28190-110">Gå til [https://protection.office.com](https://protection.office.com) og Logg på med en global administrator-eller sikkerhets administrator konto.</span><span class="sxs-lookup"><span data-stu-id="28190-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="28190-111">Velg **policy** sikker kobling i den venstre navigasjons ruten under **trussel administrasjon** \> **Safe Links** .</span><span class="sxs-lookup"><span data-stu-id="28190-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="28190-112">Velg policyen i **policyene som gjelder for hele organisasjonen** , og klikk **Rediger** .</span><span class="sxs-lookup"><span data-stu-id="28190-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="28190-113">Aktiver **Bruk sikre koblinger til meldinger som sendes i organisasjonen** under **Innstillinger** .</span><span class="sxs-lookup"><span data-stu-id="28190-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
