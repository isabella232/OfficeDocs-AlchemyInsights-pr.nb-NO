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
ms.openlocfilehash: 0d20f7bcffa3be43fc6186a938bf4a7338722f5cd225b860da6357398db26a69
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080755"
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
