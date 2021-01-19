---
title: Problemer med pålogging til programmer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901331"
---
# <a name="issues-signing-in-to-applications"></a>Problemer med pålogging til programmer

Hvis du vil finne årsaken eller diagnostisere problemer som er relatert til bruker pålogging, utfører du følgende trinn:

1. Start [påloggings diagnosen](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Finn hendelsen for å analysere ved å angi opplysningene du har om brukeren, programmet, påloggings tidspunktet, forespørsels-ID-en eller korrelasjons-IDen.
3. Se gjennom diagnose resultatene som viser informasjon om hva som skjedde og hvilke handlinger du kan utføre for å gjøre endringer, hvis det er nødvendig med endringer.

Nedenfor finner du noen vanlige problemer som kan oppstå når du logger deg på programmer:

1. Du eller brukeren **har fullført en Azure ad-pålogging, men det vises en uventet melding** – se artiklene om [uventet samtykke melding når du logger på et program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) og [uventet feil når du samtykker i et program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Du eller en bruker **har logget seg på et program direkte, men kan ikke logge på den fra en deeplink på den egen definerte portalen eller i Access-panelet**: se [Feilsøke problemer med å logge seg på et program fra Azure ad mine apper](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Du eller en bruker **har fullført en Azure ad-pålogging, men programmet viser en feil melding og lar ikke brukeren fullføre påloggings flyten**: problemet er at appen ikke godtok svaret som Azure ad har utstedt. Følg [disse trinnene](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) for å feilsøke.
4. Du eller en bruker **kan ikke logge på et ikke-galleri program som er konfigurert for enkel pålogging for passord**: Følg rettledningen i [disse trinnene](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) for å feilsøke.
5. Du eller en bruker **kan ikke logge seg på et Azure ad Gallery-program konfigurert for enkel pålogging for passord**: Følg [disse trinnene](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) for å feilsøke.
6. Du eller en bruker **kan ikke logge på et Microsoft-program**: Følg [disse trinnene](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) for å feilsøke.
7. Du eller en bruker **kan ikke logge på et ikke-galleri program som er konfigurert for delt enkel pålogging**: Følg [denne Fremgangs måten](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) for å feilsøke.
8. Du eller en bruker **kan ikke logge på et Azure ad Gallery-program som er konfigurert for delt enkel pålogging**: Følg [disse trinnene](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) for å feilsøke.
9. Du eller en bruker **kan ikke logge på et tilpasset program** som er utviklet: Følg [disse trinnene](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) for å feilsøke.
10. Du eller en bruker **kan ikke logge på et lokalt program ved hjelp av proxyen for Azure ad-program**: Følg [disse trinnene](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) for å feilsøke.

