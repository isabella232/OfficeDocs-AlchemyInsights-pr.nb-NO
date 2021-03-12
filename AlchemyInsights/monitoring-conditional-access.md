---
title: Overvåke betinget tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708683"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="923dd-102">Overvåke betinget tilgang for Exchange</span><span class="sxs-lookup"><span data-stu-id="923dd-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="923dd-103">Brukere som er angitt med betinget tilgang, mottar en e-postmelding hvis de ikke oppfyller organisasjonens krav for tilgang.</span><span class="sxs-lookup"><span data-stu-id="923dd-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="923dd-104">Hvis du vil løse problemet, anbefaler vi én eller flere av følgende løsninger:</span><span class="sxs-lookup"><span data-stu-id="923dd-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="923dd-105">Hvis det antas at enheten er registrert, ber du brukeren om å gå til Firmaportal-appen og kontrollere at den vises i firmaportalen.</span><span class="sxs-lookup"><span data-stu-id="923dd-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="923dd-106">Hvis den ikke gjør det, bør brukeren registrere enheten.</span><span class="sxs-lookup"><span data-stu-id="923dd-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="923dd-107">Gå til Intune > enhetssamsvar i Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="923dd-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="923dd-108">Klikk på Enhetssamsvar under Overvåke.</span><span class="sxs-lookup"><span data-stu-id="923dd-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="923dd-109">Vis rapporten for enhetssamsvar for å kontrollere at brukerens enhet er merket som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="923dd-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="923dd-110">Gå til Intune > enhetssamsvar i Azure-portalen.</span><span class="sxs-lookup"><span data-stu-id="923dd-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="923dd-111">Klikk Policyer under Behandle.</span><span class="sxs-lookup"><span data-stu-id="923dd-111">Under Manage, click Policies.</span></span> <span data-ttu-id="923dd-112">Kontroller at brukerens enhet er tilordnet en profil i listen over samsvarspolicyer.</span><span class="sxs-lookup"><span data-stu-id="923dd-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="923dd-113">Hvis ingen profil er tilordnet, kan ikke Intune bekrefte enhetens samsvarsstatus.</span><span class="sxs-lookup"><span data-stu-id="923dd-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="923dd-114">Rediger brukerens tilordning av betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="923dd-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="923dd-115">Gå til Policyer for betinget tilgang i **Intune**  >  **i Azure-portalen.**  >  </span><span class="sxs-lookup"><span data-stu-id="923dd-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="923dd-116">Velg en policy fra listen.</span><span class="sxs-lookup"><span data-stu-id="923dd-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="923dd-117">Klikk Brukere og grupper.</span><span class="sxs-lookup"><span data-stu-id="923dd-117">Click Users and groups.</span></span>
4. <span data-ttu-id="923dd-118">Hvis du vil rette en bestemt policy mot noen, legger du dem til i Inkluder-listen.</span><span class="sxs-lookup"><span data-stu-id="923dd-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="923dd-119">Hvis du vil sikre at en person er utelatt fra policyen, legger du vedkommende til i utelatingslisten.</span><span class="sxs-lookup"><span data-stu-id="923dd-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="923dd-120">Nyttige koblinger:</span><span class="sxs-lookup"><span data-stu-id="923dd-120">Helpful links:</span></span>

[<span data-ttu-id="923dd-121">Oversikt over enhetssamsvar</span><span class="sxs-lookup"><span data-stu-id="923dd-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="923dd-122">Feilsøking av sertifiseringsinstans</span><span class="sxs-lookup"><span data-stu-id="923dd-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="923dd-123">Feilsøking av policy</span><span class="sxs-lookup"><span data-stu-id="923dd-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="923dd-124">Overvåke intune-enhetssamsvar</span><span class="sxs-lookup"><span data-stu-id="923dd-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="923dd-125">Obs! Disse trinnene er bare nyttige når du skal feilsøke Azure Active Directory-funksjonen for betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="923dd-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="923dd-126">Det er også mulig å sette en enhet i karantene for å blokkere tilgang for e-post med Exchange-policy.</span><span class="sxs-lookup"><span data-stu-id="923dd-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="923dd-127">Du finner mer informasjon om administrasjon av Exchange-enheter [her]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="923dd-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
