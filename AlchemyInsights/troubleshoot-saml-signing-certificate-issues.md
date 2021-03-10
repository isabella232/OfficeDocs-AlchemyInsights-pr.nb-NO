---
title: Feilsøke problemer med SAML-signeringssertifikatet
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694444"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>Feilsøke problemer med SAML-signeringssertifikatet

Utfør følgende anbefalte trinn for å løse problemet med SAML-signeringssertifikatet:

1. Når du legger til et virksomhetsprogram som støtter SSO, genererer Azure et sertifikat som kalles [SAML-signatursertifikatet.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) Dette sertifikatet har en utløpsdato på tre år. Hvis du vil endre utløpsdatoen for sertifikatet, kan du se Tilpasse utløpsdatoen for forbundssertifikatet og rulle [den over til et nytt sertifikat.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)
2. Azure bruker dette sertifikatet til å signere SAML-tokenene som er forespurt av programmet, og sender det over til programmet for å få en vellykket SSO. For at dette skal fullføres må du laste ned sertifikatet fra Azure Portal og sende det til programleverandøren for å fullføre SSO-prosessen.

Når denne prosessen er fullført, vil programmet klarere dette sertifikatet, og alle SAML-tokener som er signert med dette sertifikatet, godkjennes av programmet.

3. Hvis dette sertifikatet utløper, oppretter du et nytt sertifikat, oppdaterer det til programleverandøren og gjør det aktivt på Azure-siden. Hvis du vil ha mer informasjon, kan du se Fornye et [sertifikat som snart utløper.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)

> [!NOTE]
> Hvis sertifikatet utløper, blokkeres ikke brukeren.

4. [Legg til en e-postadresse for](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) varsler som skal mottas før det gjeldende sertifikatet utløper.

> [!NOTE]
> Trinn 4 er valgfritt.

5. Endre alternativene for SAML-sertifikatsignering i et program og algoritmen for sertifikatsignering. Hvis du vil ha mer informasjon, kan du se Endre alternativer for [sertifikatsignering og signeringsalgoritme.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)

