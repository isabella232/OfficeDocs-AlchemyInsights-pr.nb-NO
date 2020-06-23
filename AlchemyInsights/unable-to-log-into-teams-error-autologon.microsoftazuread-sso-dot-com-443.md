---
title: Kan ikke logge på Teams på grunn av feilen autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932037"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Kan ikke logge på Teams på grunn av feilen autologon.microsoftazuread-sso dot.com:443

Hvis sømløs enkel pålogging er aktivert som O365-godkjenning, må kanskje nettadressen autologon.microsoftazuread-sso.com legges til i intranettområdene.  Hvis den tidligere har blitt lagt til i klarerte områder og sømløs enkel pålogging er i bruk, bør den fjernes fra klarerte områder.

Hvis du vil ha mer informasjon, kan du gå igjennom [Sjekkliste for feilsøking av sømløs enkel pålogging](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Følg disse trinnene for å legge til en nettadresse i listen over intranettområder:

1. Åpne Internet Explorer ved å klikke på **Start**. Skriv inn Internet Explorer i søkeboksen, og klikk deretter på **Internet Explorer** i resultatlisten.
2. Klikk på **Verktøy**, og klikk deretter på **Alternativer for Internett**.
3. Klikk på **Sikkerhet**-fanen.
4. Nå klikker du på **Lokalt intranett** og deretter klikker på **Områder**-knappen og **Avansert**-knappen.
5. Skriv inn nettadressen til nettstedet, og klikk på **Legg til**.
6. Når du er ferdig, klikker du på **Lukk**.

Hvis du vil ha mer informasjon, kan du se [Dokumentasjon for å distribuere sømløs enkel pålogging for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (inkluderer policybasert prosess for å legge til en nettadresse i intranettområder i trinn 3).
