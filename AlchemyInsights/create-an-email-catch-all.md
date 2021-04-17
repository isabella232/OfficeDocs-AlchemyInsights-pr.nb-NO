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
# <a name="create-an-email-catch-all"></a>Opprette en fangst for e-post alle

Bruk av en fangst frarådes på det sterkeste. Det er bedre å sende en retur tilbake til avsenderen slik at avsenderne vet at meldingen ikke kunne leveres som adressert, slik at de kan gjøre noe. Du kan også begrense den overvåkede postboksen slik at den bare fanger opp tidligere gyldige e-postadresser. 

Alle postbokser som fanges opp, mottar mye søppelpost og kan etter hvert fylles ut hvis de ikke overvåkes nøye. (Det finnes mottaksgrenser.) 

Hvis du bestemmer deg for å fortsette, følger du disse trinnene:

1. Opprett en dynamisk distribusjonsgruppe & «Alle mottakertyper».

2. Opprett en dedikert postboks for å hente e-postmeldinger, for eksempel catchall@domain.com.

3. Angi DomainType til InternalRelay for det bestemte domenet. Hvis du senere fjerner fangsten alle, må du angi domenet tilbake til Autoritativ.

4. Opprett en transportregel for e-postflyt på følgende måte:

    - Hvis avsenderen er utenfor organisasjonen
    - Omdiriger meldingen til Catchall@domain.com
    - Bortsett fra hvis mottakeren er medlem av allusers@domain.com (Distribusjonsgruppe inneholder alle medlemmer)
    - Sikre at nye postbokser legges til i den dynamiske distribusjonsgruppen
