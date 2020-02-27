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
# <a name="create-an-email-catch-all"></a>Opprett en e-postfangst alle

Bruk av en fangst alt er sterkt motløs. Det er bedre å gi en sprett tilbake til avsenderen som lar avsendere vite at meldingen deres ikke kunne leveres som adressert, slik at de kan iverksette tiltak. Du kan også begrense den overvåkede postboksen til bare å fange tidligere gyldige e-postadresser. 

Enhver fangst alle postkasse vil motta en god del spam og kan til slutt fylle hvis ikke nøye overvåket. (Det er mottaksgrenser.) 

Hvis du bestemmer deg for å fortsette, gjør du følgende:

1. Opprett en dynamisk distribusjonsgruppe & inkludere "Alle mottakertyper".

2. Opprett en dedikert postboks for å fange e-postmeldinger, for eksempel catchall@domain.com.

3. For det bestemte domenet setter du DomainType til "InternalRelay". Hvis du senere fjerner fangsten alle, må du passe på å sette domenet tilbake til Autoritativ.

4. Opprett en mailflow-transportregel på følgende måte:

    - Hvis avsenderen er "Utenfor organisasjonen"
    - Omdirigere meldingen til Catchall@domain.com
    - Bortsett fra hvis mottakeren er medlem av allusers@domain.com (Distribusjonsgruppe inneholder alle medlemmer)
    - Kontroller at nye postbokser legges til i dynamisk distribusjonsgruppe
