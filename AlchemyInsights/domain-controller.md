---
title: Domene kontroller
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901308"
---
# <a name="domain-controller"></a>Domene kontroller

**Kan ikke aktivere AAD-DS eller distribusjon mislykkes**

Hvis du vil løse problemet med at Azure AD Domain Service (AAD-DS) ikke aktiveres eller ikke kan distribueres, utfører du følgende trinn:

1. Hvis du bruker et virtuelt nettverk som allerede finnes, må du kontrollere NSG for regler som blokkerer porter som er nødvendige for å synkronisere i AAD-DS i portalen https://aka.ms/aadds-networking .
2. Kontroller om feil meldingen er besvart i denne veiledningen for feil søking som er tilgjengelig i  https://aka.ms/aadds-troubleshoot-enable .
3. Prøv å distribuere Azure AD Domain Services i et nytt virtuelt nettverk.
4. Følg instruksjonene i komme i gang med hvordan du distribuerer AAD-DS, som er tilgjengelig i [opplæring for å opprette Azure ad Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. Hvis du har problemer med å distribuere Azure AD Domain Services, kan du se [Feilsøke Azure ad Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) for å løse vanlige feil for å få ting til å fungere på nytt. 

**Kan ikke deaktivere AAD-DS**

AAD-DS kan ikke stanses midlertidig. Hvis du vil slutte å bruke det forvaltede domenet, må det slettes.

Hvis det oppstår problemer, kan du løse vanlige feil meldinger og for å få de tilknyttede feil søkings trinnene for å hjelpe deg med å kjøre dem igjen, se [Feilsøke Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
