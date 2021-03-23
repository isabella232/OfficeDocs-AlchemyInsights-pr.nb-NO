---
title: Beskyttelse mot backscatter-angrep
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036077"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="8545f-102">Beskyttelse mot backscatter-angrep</span><span class="sxs-lookup"><span data-stu-id="8545f-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="8545f-103">Backscatter er rapporter om manglende levering (også kalt NDR-er eller returmeldinger) du mottar for meldinger du ikke har sendt.</span><span class="sxs-lookup"><span data-stu-id="8545f-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="8545f-104">Søppelpostsendere forfalsket **Fra-adressen** til meldingene sine, og de bruker ofte ekte e-postadresser til å gi troverdighet til meldingene sine.</span><span class="sxs-lookup"><span data-stu-id="8545f-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="8545f-105">Så når søppelpostsendere uunngåelig sender meldinger til ikke-eksisterende mottakere, blir mål-e-postserveren i hovedsak lurt til å returnere meldingen som ikke kan leveres, i en NDR til den forfalskede avsenderen i **Fra:-adressen.**</span><span class="sxs-lookup"><span data-stu-id="8545f-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="8545f-106">Du finner mer informasjon i [Backscatter i EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="8545f-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="8545f-107">**Aktivere backscatter-beskyttelse**</span><span class="sxs-lookup"><span data-stu-id="8545f-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="8545f-108">Hvis du vil aktivere Backscatter-beskyttelse, følger du banen nedenfor.</span><span class="sxs-lookup"><span data-stu-id="8545f-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="8545f-109">**protection.office.com > Policy > Policy > Antispam > Velg policyen for søppelpostfilter og Rediger policy > Egenskaper for søppelpost > Merk som søppelpost > NDR-tilbakevindu > Angi den til På**</span><span class="sxs-lookup"><span data-stu-id="8545f-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="8545f-110">Hvis du mener at en konto er kompromittert, kan du se følgende:</span><span class="sxs-lookup"><span data-stu-id="8545f-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="8545f-111">Svare på en kompromittert e-postkonto</span><span class="sxs-lookup"><span data-stu-id="8545f-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="8545f-112">Fjerne blokkerte brukere fra portalen begrensede brukere i Office 365</span><span class="sxs-lookup"><span data-stu-id="8545f-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



