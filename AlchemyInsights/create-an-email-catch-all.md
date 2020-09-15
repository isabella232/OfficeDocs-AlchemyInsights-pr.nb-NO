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
# <a name="create-an-email-catch-all"></a>Opprette en e-postcatch

Det frarådes å bruke en catch-alt. Det er bedre å gi en sprett tilbake til avsenderen som lar avsendere få vite at meldingen ikke kan leveres som adressert, slik at de kan gjøre noe. Du kan også begrense den overvåkede post boksen til bare å fange opp tidligere gyldige e-postadresser. 

Alle Catch-all post boks vil motta en god del av søppel post og kan til og med fylles ut hvis det ikke er tettere. (Det finnes mottaks begrensninger) 

Hvis du vil fortsette, følger du disse trinnene:

1. Opprett en dynamisk distribusjons gruppe & inkludere alle mottaker typer.

2. Opprett en egen post boks for å fange opp e-postmeldinger, for eksempel catchall@domain.com.

3. For det spesifikke domenet setter du DomainType til «InternalRelay». Hvis du senere fjerner oppsamlingen, må du passe på å sette domenet tilbake til autoritativ.

4. Opprett en Mailflow-transport regel på følgende måte:

    - Hvis avsenderen er «utenfor organisasjonen»
    - Omadresser meldingen til Catchall@domain.com
    - Unntatt hvis mottakeren er medlem av allusers@domain.com (distribusjons gruppe inneholder alle medlemmer)
    - Pass på å validere at nye post bokser legges til i den dynamiske distribusjons gruppen
