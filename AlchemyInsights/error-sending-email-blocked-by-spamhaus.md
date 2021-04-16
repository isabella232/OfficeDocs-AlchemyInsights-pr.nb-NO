---
title: Feil under sending av e-post blokkert av SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813733"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="bd7a1-102">Feil under sending av e-post: Klientvert blokkert ved hjelp av Spamhaus</span><span class="sxs-lookup"><span data-stu-id="bd7a1-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="bd7a1-103">IP-adressen som sendte meldingen, er på en blokkeringsliste som eies av [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="bd7a1-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="bd7a1-104">Årsaker til å bli blokkert av Spamhaus omfatter kompromitterte kontoer, kompromitterte maskiner som deler en offentlig IP-adresse og Policyer for Internett-leverandør (ISP).</span><span class="sxs-lookup"><span data-stu-id="bd7a1-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="bd7a1-105">Mulige løsninger er:</span><span class="sxs-lookup"><span data-stu-id="bd7a1-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="bd7a1-106">For blokkerte innkommende meldinger der du kontrollerer kilde-e-postserveren, må du finne årsaken og fjerne blokkeringen fra Spamhaus-nettstedet.</span><span class="sxs-lookup"><span data-stu-id="bd7a1-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="bd7a1-107">For blokkerte innkommende meldinger der kilde-IP-adressen tilhører noen andre, må adresseeieren fjerne blokkeringen fra Spamhaus-nettstedet.</span><span class="sxs-lookup"><span data-stu-id="bd7a1-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="bd7a1-108">Hvis IP-adressen er på blokkeringslisten for policy (PBL), kan eieren tilordne en annen statisk IP-adresse eller fjerne adressen fra PBL.</span><span class="sxs-lookup"><span data-stu-id="bd7a1-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="bd7a1-109">For blokkerte utgående meldinger fra domenet som er koblet til Microsoft, kan du få denne feilmeldingen hvis meldingene rutes gjennom en tredjepartstjeneste.</span><span class="sxs-lookup"><span data-stu-id="bd7a1-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="bd7a1-110">Du kan bruke et WHOIS-oppslagsverktøy til å finne eieren av den blokkerte IP-adressen.</span><span class="sxs-lookup"><span data-stu-id="bd7a1-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
