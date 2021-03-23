---
title: Arbeide med godkjenningsbiblioteker
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035826"
---
# <a name="working-with-authentication-libraries"></a>Arbeide med godkjenningsbiblioteker

Hvis du vil løse problemet med Microsoft Authentication Library (MSAL), utfører du følgende anbefalte trinn:

1. **Arbeide med MSAL:** [Godkjenningsbiblioteker for Microsoft-identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – Denne artikkelen viser støtte for Microsoft Authentication Library for flere programtyper. Den inneholder koblinger til kildekoden for biblioteket. hvor du får pakken for appens prosjekt; og om biblioteket støtter bruker pålogging (godkjenning), tilgang til beskyttede web-API-er (autorisasjon) eller begge deler.

2. **Feilsøkingsgodkjenning:** MSAL støtter flere godkjenningsflyter for bruk i ulike programscenarioer. Avhengig av hvordan klientprogrammet er bygd, kan MSAL bruke én eller flere av godkjenningsflytene som støttes av Microsoft-identitetsplattformen. Disse flytene kan produsere flere typer tokener og autorisasjonskoder, og kreve ulike tokener for å få dem til å fungere.

3. **Tilgangstokener:** [Tilgangstokener for Microsoft-identitetsplattform](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Finn ut hvordan API-en kan validere og bruke påstandene i et tilgangstoken. All dokumentasjon i denne artikkelen, unntatt der det er notert, gjelder bare for tokener utstedt for API-er du har registrert. Det gjelder ikke tokener utstedt for Microsoft-eide API-er, og disse tokenene kan heller ikke brukes til å validere hvordan Microsoft-identitetsplattformen vil utstede tokener for en API du oppretter.

**Slutt på støtte for Azure Active Directory Authentication Library (ADAL)**

- **Fra og med 30. juni 2020** legger vi ikke lenger til noen nye funksjoner i ADAL og Azure AD Graph. Vi vil fortsette å tilby teknisk støtte og sikkerhetsoppdateringer, men vi vil ikke lenger tilby funksjonsoppdateringer.
- **Fra og med 30. juni 2022** avslutter vi støtte for ADAL og Azure AD Graph og vil ikke lenger tilby teknisk støtte eller sikkerhetsoppdateringer.
- Apper som bruker ADAL på eksisterende OS-versjoner, vil fortsette å fungere etter dette tidspunktet, men vil ikke få teknisk *støtte eller sikkerhetsoppdateringer.*
- Apper som bruker Azure AD Graph etter dette tidspunktet, mottar kanskje ikke lenger svar fra Azure AD Graph-endepunktet.

**ADAL-overføring**

- Vi anbefaler å oppdatere til MSAL, som har de nyeste funksjonene og sikkerhetsoppdateringene.
- Hvis du bruker Microsoft-apper, må du vite at Microsoft er i ferd med å overføre appene til MSAL innen tidsfristen for kundestøtten utløper, slik at de vil dra nytte av MSAL sine pågående sikkerhets- og funksjonsforbedringer.

1. [Les vanlige spørsmål om ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [Lær om hvordan du overfører apper per plattform.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance)
3. Hvis du har flere spørsmål etter å ha lest veiledningen for appens plattform, kan du publisere på [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) med koden [azure-ad-adal-deprecation] eller åpne et problem i bibliotekets GitHub-repositorium. Se [språk- og rammeverkdelen i](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) **MSAL-oversiktsartikkelen** for koblinger til hvert biblioteks repo.
4. Hvis du trenger hjelp til å forstå hvilke av **appene som bruker ADAL,** anbefaler vi at du ser gjennom kildekoden til alle appene dine. Hvis det er aktuelt, kan du ta kontakt med uavhengige programvareleverandører (ISV-er) eller appleverandører. Microsoft Kundestøtte kan også gi deg en liste over alle ADAL-appene i tenanten som ikke er fra Microsoft.







