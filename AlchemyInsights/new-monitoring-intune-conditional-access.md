---
title: Overvåke Betinget tilgang med Intune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427924"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="6d8ae-102">Overvåke Betinget tilgang med Intune</span><span class="sxs-lookup"><span data-stu-id="6d8ae-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="6d8ae-103">Brukere som er angitt med betinget tilgang, mottar en e-postmelding hvis de ikke oppfyller organisasjonens krav for tilgang.</span><span class="sxs-lookup"><span data-stu-id="6d8ae-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="6d8ae-104">Hvis du vil løse problemet, anbefaler vi én eller flere av følgende løsninger:</span><span class="sxs-lookup"><span data-stu-id="6d8ae-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="6d8ae-105">Hvis det antas at enheten er registrert, ber du brukeren om å gå til Firmaportal-appen og kontrollere at den vises i firmaportalen.</span><span class="sxs-lookup"><span data-stu-id="6d8ae-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="6d8ae-106">Hvis den ikke gjør det, må brukeren registrere enheten.</span><span class="sxs-lookup"><span data-stu-id="6d8ae-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="6d8ae-107">Gå til Enhetssamsvar for **Intune**  >  **i Azure-portalen.**</span><span class="sxs-lookup"><span data-stu-id="6d8ae-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="6d8ae-108">Hvis du vil vise rapporten om enhetssamsvar for å kontrollere at brukerens enhet er merket som kompatibel, klikker du Enhetssamsvar **under** **Skjerm.**</span><span class="sxs-lookup"><span data-stu-id="6d8ae-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="6d8ae-109">Gå til Enhetssamsvar for **Intune**  >  **i Azure-portalen.**</span><span class="sxs-lookup"><span data-stu-id="6d8ae-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="6d8ae-110">Klikk **Policyer** under **Behandle.**</span><span class="sxs-lookup"><span data-stu-id="6d8ae-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="6d8ae-111">Kontroller at brukerens enhet er tilordnet en profil i listen over samsvarspolicyer.</span><span class="sxs-lookup"><span data-stu-id="6d8ae-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="6d8ae-112">Hvis ingen profil er tilordnet, kan ikke Intune bekrefte enhetens samsvarsstatus.</span><span class="sxs-lookup"><span data-stu-id="6d8ae-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="6d8ae-113">Rediger brukerens tilordning av betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="6d8ae-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="6d8ae-114">Gå til **Intune-policyer** for betinget tilgang i Azure-portalen, velg en policy fra listen, og klikk  >    >  Brukere **og grupper.**</span><span class="sxs-lookup"><span data-stu-id="6d8ae-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="6d8ae-115">Hvis du vil rette en bestemt policy mot noen, legger du dem til **i Inkluder-listen.**</span><span class="sxs-lookup"><span data-stu-id="6d8ae-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="6d8ae-116">Hvis du vil sikre at en person er utelatt fra policyen, legger du vedkommende til i **utelatingslisten.**</span><span class="sxs-lookup"><span data-stu-id="6d8ae-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="6d8ae-117">**Nyttige koblinger:**</span><span class="sxs-lookup"><span data-stu-id="6d8ae-117">**Helpful links:**</span></span>

- [<span data-ttu-id="6d8ae-118">Oversikt over enhetssamsvar</span><span class="sxs-lookup"><span data-stu-id="6d8ae-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="6d8ae-119">Feilsøking av sertifiseringsinstans</span><span class="sxs-lookup"><span data-stu-id="6d8ae-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="6d8ae-120">Feilsøking av policy</span><span class="sxs-lookup"><span data-stu-id="6d8ae-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="6d8ae-121">Overvåke intune-enhetssamsvar</span><span class="sxs-lookup"><span data-stu-id="6d8ae-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="6d8ae-122">Disse trinnene er bare nyttige når du skal feilsøke Azure Active Directory-funksjonen betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="6d8ae-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="6d8ae-123">Det er også mulig å sette en enhet i karantene for å blokkere tilgangen til e-post med Exchange-policy.</span><span class="sxs-lookup"><span data-stu-id="6d8ae-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="6d8ae-124">Du finner mer informasjon om administrasjon av Exchange-enheter [**her.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))</span><span class="sxs-lookup"><span data-stu-id="6d8ae-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
