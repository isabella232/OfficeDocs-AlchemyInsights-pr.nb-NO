---
title: Opprette en e-postcatch
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712995"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="f45e5-102">Opprette en e-postcatch</span><span class="sxs-lookup"><span data-stu-id="f45e5-102">Create an email catch all</span></span>

<span data-ttu-id="f45e5-103">Det frarådes å bruke en catch-alt.</span><span class="sxs-lookup"><span data-stu-id="f45e5-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="f45e5-104">Det er bedre å gi en sprett tilbake til avsenderen som lar avsendere få vite at meldingen ikke kan leveres som adressert, slik at de kan gjøre noe.</span><span class="sxs-lookup"><span data-stu-id="f45e5-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="f45e5-105">Du kan også begrense den overvåkede post boksen til bare å fange opp tidligere gyldige e-postadresser.</span><span class="sxs-lookup"><span data-stu-id="f45e5-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="f45e5-106">Alle Catch-all post boks vil motta en god del av søppel post og kan til og med fylles ut hvis det ikke er tettere.</span><span class="sxs-lookup"><span data-stu-id="f45e5-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="f45e5-107">(Det finnes mottaks begrensninger)</span><span class="sxs-lookup"><span data-stu-id="f45e5-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="f45e5-108">Hvis du vil fortsette, følger du disse trinnene:</span><span class="sxs-lookup"><span data-stu-id="f45e5-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="f45e5-109">Opprett en dynamisk distribusjons gruppe & inkludere alle mottaker typer.</span><span class="sxs-lookup"><span data-stu-id="f45e5-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="f45e5-110">Opprett en egen post boks for å fange opp e-postmeldinger, for eksempel catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="f45e5-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="f45e5-111">For det spesifikke domenet setter du DomainType til «InternalRelay».</span><span class="sxs-lookup"><span data-stu-id="f45e5-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="f45e5-112">Hvis du senere fjerner oppsamlingen, må du passe på å sette domenet tilbake til autoritativ.</span><span class="sxs-lookup"><span data-stu-id="f45e5-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="f45e5-113">Opprett en Mailflow-transport regel på følgende måte:</span><span class="sxs-lookup"><span data-stu-id="f45e5-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="f45e5-114">Hvis avsenderen er «utenfor organisasjonen»</span><span class="sxs-lookup"><span data-stu-id="f45e5-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="f45e5-115">Omadresser meldingen til Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="f45e5-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="f45e5-116">Unntatt hvis mottakeren er medlem av allusers@domain.com (distribusjons gruppe inneholder alle medlemmer)</span><span class="sxs-lookup"><span data-stu-id="f45e5-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="f45e5-117">Pass på å validere at nye post bokser legges til i den dynamiske distribusjons gruppen</span><span class="sxs-lookup"><span data-stu-id="f45e5-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
