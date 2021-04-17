---
title: Opprette en fangst for e-post alle
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816209"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="8a146-102">Opprette en fangst for e-post alle</span><span class="sxs-lookup"><span data-stu-id="8a146-102">Create an email catch all</span></span>

<span data-ttu-id="8a146-103">Bruk av en fangst frarådes på det sterkeste.</span><span class="sxs-lookup"><span data-stu-id="8a146-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="8a146-104">Det er bedre å sende en retur tilbake til avsenderen slik at avsenderne vet at meldingen ikke kunne leveres som adressert, slik at de kan gjøre noe.</span><span class="sxs-lookup"><span data-stu-id="8a146-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="8a146-105">Du kan også begrense den overvåkede postboksen slik at den bare fanger opp tidligere gyldige e-postadresser.</span><span class="sxs-lookup"><span data-stu-id="8a146-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="8a146-106">Alle postbokser som fanges opp, mottar mye søppelpost og kan etter hvert fylles ut hvis de ikke overvåkes nøye.</span><span class="sxs-lookup"><span data-stu-id="8a146-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="8a146-107">(Det finnes mottaksgrenser.)</span><span class="sxs-lookup"><span data-stu-id="8a146-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="8a146-108">Hvis du bestemmer deg for å fortsette, følger du disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="8a146-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="8a146-109">Opprett en dynamisk distribusjonsgruppe & «Alle mottakertyper».</span><span class="sxs-lookup"><span data-stu-id="8a146-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="8a146-110">Opprett en dedikert postboks for å hente e-postmeldinger, for eksempel catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="8a146-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="8a146-111">Angi DomainType til InternalRelay for det bestemte domenet.</span><span class="sxs-lookup"><span data-stu-id="8a146-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="8a146-112">Hvis du senere fjerner fangsten alle, må du angi domenet tilbake til Autoritativ.</span><span class="sxs-lookup"><span data-stu-id="8a146-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="8a146-113">Opprett en transportregel for e-postflyt på følgende måte:</span><span class="sxs-lookup"><span data-stu-id="8a146-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="8a146-114">Hvis avsenderen er utenfor organisasjonen</span><span class="sxs-lookup"><span data-stu-id="8a146-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="8a146-115">Omdiriger meldingen til Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="8a146-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="8a146-116">Bortsett fra hvis mottakeren er medlem av allusers@domain.com (Distribusjonsgruppe inneholder alle medlemmer)</span><span class="sxs-lookup"><span data-stu-id="8a146-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="8a146-117">Sikre at nye postbokser legges til i den dynamiske distribusjonsgruppen</span><span class="sxs-lookup"><span data-stu-id="8a146-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
