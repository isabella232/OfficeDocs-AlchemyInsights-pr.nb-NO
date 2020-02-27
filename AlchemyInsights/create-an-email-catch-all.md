---
title: Opprett en e-postfangst alle
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286201"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="0d429-102">Opprett en e-postfangst alle</span><span class="sxs-lookup"><span data-stu-id="0d429-102">Create an email catch all</span></span>

<span data-ttu-id="0d429-103">Bruk av en fangst alt er sterkt motløs.</span><span class="sxs-lookup"><span data-stu-id="0d429-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="0d429-104">Det er bedre å gi en sprett tilbake til avsenderen som lar avsendere vite at meldingen deres ikke kunne leveres som adressert, slik at de kan iverksette tiltak.</span><span class="sxs-lookup"><span data-stu-id="0d429-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="0d429-105">Du kan også begrense den overvåkede postboksen til bare å fange tidligere gyldige e-postadresser.</span><span class="sxs-lookup"><span data-stu-id="0d429-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="0d429-106">Enhver fangst alle postkasse vil motta en god del spam og kan til slutt fylle hvis ikke nøye overvåket.</span><span class="sxs-lookup"><span data-stu-id="0d429-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="0d429-107">(Det er mottaksgrenser.)</span><span class="sxs-lookup"><span data-stu-id="0d429-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="0d429-108">Hvis du bestemmer deg for å fortsette, gjør du følgende:</span><span class="sxs-lookup"><span data-stu-id="0d429-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="0d429-109">Opprett en dynamisk distribusjonsgruppe & inkludere "Alle mottakertyper".</span><span class="sxs-lookup"><span data-stu-id="0d429-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="0d429-110">Opprett en dedikert postboks for å fange e-postmeldinger, for eksempel catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="0d429-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="0d429-111">For det bestemte domenet setter du DomainType til "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="0d429-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="0d429-112">Hvis du senere fjerner fangsten alle, må du passe på å sette domenet tilbake til Autoritativ.</span><span class="sxs-lookup"><span data-stu-id="0d429-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="0d429-113">Opprett en mailflow-transportregel på følgende måte:</span><span class="sxs-lookup"><span data-stu-id="0d429-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="0d429-114">Hvis avsenderen er "Utenfor organisasjonen"</span><span class="sxs-lookup"><span data-stu-id="0d429-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="0d429-115">Omdirigere meldingen til Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="0d429-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="0d429-116">Bortsett fra hvis mottakeren er medlem av allusers@domain.com (Distribusjonsgruppe inneholder alle medlemmer)</span><span class="sxs-lookup"><span data-stu-id="0d429-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="0d429-117">Kontroller at nye postbokser legges til i dynamisk distribusjonsgruppe</span><span class="sxs-lookup"><span data-stu-id="0d429-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
