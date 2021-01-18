---
title: Konfigurere Domain service
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885693"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>Kan ikke aktivere AAD-DS eller distribusjon mislykkes

Hvis du vil løse problemet med at Azure AD Domain Service (AAD-DS) ikke aktiveres eller ikke kan distribueres, utfører du følgende trinn:

1. Hvis du bruker et virtuelt nettverk som allerede finnes, må du kontrollere NSG for regler som blokkerer porter som er nødvendige for å synkronisere i AAD-DS i portalen https://aka.ms/aadds-networking .
2. Kontroller om feil meldingen er besvart i denne veiledningen for feil søking som er tilgjengelig i  https://aka.ms/aadds-troubleshoot-enable .
3. Prøv å distribuere Azure AD Domain Services i et nytt virtuelt nettverk.
4. Følg instruksjonene i komme i gang med hvordan du distribuerer AAD-DS: [opprette og konfigurere AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Hvis du har problemer med å distribuere Azure AD Domain Services, kan du se [Feilsøke Azure ad Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) for å løse vanlige feil for å få ting til å fungere på nytt. 

**Kan ikke deaktivere AAD-DS**

AAD-DS kan ikke stanses midlertidig. Hvis du vil slutte å bruke det forvaltede domenet, må det slettes.
Hvis du vil slette det administrerte domenet, kan du se [slette AAD Domain service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



