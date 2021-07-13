---
title: Utgående videresendingsutvalg
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381858"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="3396a-102">Utgående videresendingsutvalg</span><span class="sxs-lookup"><span data-stu-id="3396a-102">Outbound relay pool</span></span>

<span data-ttu-id="3396a-103">Microsoft gjør noen endringer i konfigurasjonen for videresending eller videresending av e-post via Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3396a-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="3396a-104">Meldinger i bestemte scenarier videresendes eller videresendes gjennom Microsoft 365 ved hjelp av et spesielt videresendingsutvalg.</span><span class="sxs-lookup"><span data-stu-id="3396a-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="3396a-105">Meldinger som sendes ved hjelp av videresendingsutvalget, kan ende opp i mottakerens søppelpostmappe.</span><span class="sxs-lookup"><span data-stu-id="3396a-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="3396a-106">Hvis du vil ha mer informasjon, kan du [se Utgående leveringsutvalg](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="3396a-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="3396a-107">Hvis du vil unngå et scenario ved hjelp av videresendingsutvalget, må du kontrollere at videresendte/videresendte meldinger oppfyller ett av følgende kriterier:</span><span class="sxs-lookup"><span data-stu-id="3396a-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="3396a-108">Den utgående avsenderen er et godtatt domene for leieren.</span><span class="sxs-lookup"><span data-stu-id="3396a-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="3396a-109">SpF (Sender Policy Framework) sendes når meldingen kommer til Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3396a-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="3396a-110">DomainKeys Identified Mail (DKIM) på P2-avsenderdomenet sendes når meldingen kommer til Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="3396a-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="3396a-111">Meldinger som oppfyller vilkårene ovenfor, videresendes ikke gjennom videresendingsutvalget.</span><span class="sxs-lookup"><span data-stu-id="3396a-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="3396a-112">Hvis MX-posten for domenet peker til en tredjeparts eller lokal server, kan du bruke forbedret filtrering for å sikre at SPF-valideringen er riktig for inngående e-post og for å unngå å sende e-post gjennom videresendingsutvalget.</span><span class="sxs-lookup"><span data-stu-id="3396a-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="3396a-113">**Hvordan kan vi se om vi påvirkes av videresendingsutvalget?**</span><span class="sxs-lookup"><span data-stu-id="3396a-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="3396a-114">Hvis videresendte eller videresendte e-postmeldinger bruker et av vilkårene ovenfor, sendes ikke meldinger gjennom videresendingsutvalget.</span><span class="sxs-lookup"><span data-stu-id="3396a-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="3396a-115">Hvis en melding sendes via et videresendingsutvalg, er imidlertid den utgående server-IP-adressen i området 40.95.0.0/16, og det utgående servernavnet inneholder **rly** i navnet.</span><span class="sxs-lookup"><span data-stu-id="3396a-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

