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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366437"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="90a3a-102">Overvåke betinget tilgang for Exchange</span><span class="sxs-lookup"><span data-stu-id="90a3a-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="90a3a-103">Brukere som er rettet mot betinget tilgang, mottar en e-postvarsling hvis de ikke oppfyller organisasjonens tilgangs krav.</span><span class="sxs-lookup"><span data-stu-id="90a3a-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="90a3a-104">Vi anbefaler en eller flere av følgende løsninger for å løse:</span><span class="sxs-lookup"><span data-stu-id="90a3a-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="90a3a-105">Hvis enheten er Presumed for å bli registrert, ber du brukeren om å gå til Firmaportal-appen og kontrollere at den vises i firma portalen.</span><span class="sxs-lookup"><span data-stu-id="90a3a-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="90a3a-106">Hvis den ikke gjør det, skal brukeren registrere enheten.</span><span class="sxs-lookup"><span data-stu-id="90a3a-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="90a3a-107">I Azure-portalen går du til Intune > enhets samsvar.</span><span class="sxs-lookup"><span data-stu-id="90a3a-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="90a3a-108">Under skjerm klikk enhets samsvar.</span><span class="sxs-lookup"><span data-stu-id="90a3a-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="90a3a-109">Vis samsvars rapporten for enheten for å bekrefte at brukerens enhet er merket som kompatibel.</span><span class="sxs-lookup"><span data-stu-id="90a3a-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="90a3a-110">I Azure-portalen går du til Intune > enhets samsvar.</span><span class="sxs-lookup"><span data-stu-id="90a3a-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="90a3a-111">Klikk policyer under behandle.</span><span class="sxs-lookup"><span data-stu-id="90a3a-111">Under Manage, click Policies.</span></span> <span data-ttu-id="90a3a-112">Kontroller at en profil er tilordnet til brukerens enhet i listen over samsvars policyer.</span><span class="sxs-lookup"><span data-stu-id="90a3a-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="90a3a-113">Hvis ingen profil er tilordnet, vil ikke Intune kunne bekrefte enhetens samsvars status.</span><span class="sxs-lookup"><span data-stu-id="90a3a-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="90a3a-114">Rediger brukerens tilordningen for betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="90a3a-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="90a3a-115">Gå til **Intune**-policyer for  >  **betinget tilgang**i Azure-portalen  >  **Policies**.</span><span class="sxs-lookup"><span data-stu-id="90a3a-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="90a3a-116">Velg en policy fra listen.</span><span class="sxs-lookup"><span data-stu-id="90a3a-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="90a3a-117">Klikk brukere og grupper.</span><span class="sxs-lookup"><span data-stu-id="90a3a-117">Click Users and groups.</span></span>
4. <span data-ttu-id="90a3a-118">Hvis du vil angi en bestemt policy for noen, kan du legge dem til i inkluderings listen.</span><span class="sxs-lookup"><span data-stu-id="90a3a-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="90a3a-119">Hvis du vil sikre at en person utelates fra policyen, legger du dem til i ekskluderings listen.</span><span class="sxs-lookup"><span data-stu-id="90a3a-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="90a3a-120">Nyttige koblinger:</span><span class="sxs-lookup"><span data-stu-id="90a3a-120">Helpful links:</span></span>

[<span data-ttu-id="90a3a-121">Oversikt over enhets samsvar</span><span class="sxs-lookup"><span data-stu-id="90a3a-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="90a3a-122">Feilsøke sertifiserings instans</span><span class="sxs-lookup"><span data-stu-id="90a3a-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="90a3a-123">Feil søkings policy</span><span class="sxs-lookup"><span data-stu-id="90a3a-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="90a3a-124">Overvåke enhets samsvar for Intune</span><span class="sxs-lookup"><span data-stu-id="90a3a-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="90a3a-125">Obs! disse trinnene er bare nyttige ved feil søking av Azure Active Directory-funksjonen betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="90a3a-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="90a3a-126">Det er også mulig å karantene en enhet som blokkerer e-posttilgang med Exchange-policy.</span><span class="sxs-lookup"><span data-stu-id="90a3a-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="90a3a-127">Du finner mer informasjon om administrasjon av Exchange-enheter [her](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="90a3a-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
