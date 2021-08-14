---
title: Problem med AAD Koble til Tilstand
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923761"
---
# <a name="problem-with-aad-connect-health"></a>Problem med AAD Koble til Tilstand

- Kontroller at du er autorisert til å utføre operasjonen. Globale administratorer har tilgang som standard. I tillegg kan du bruke rollebasert [tilgangskontroll til](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) å delegere registreringstillatelse til bidragsyter.
- Kontroller at de nødvendige endepunktene er aktivert, og ikke blokkert på grunn av brannmuren. Hvis du vil ha mer informasjon, kan du se [krav](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registreringen kan mislykkes på grunn av at utgående kommunikasjon blir utsatt for SSL-inspeksjon av nettverkslaget.
- Kontroller at du har bekreftet varslingsinnstillingene for Azure AD Koble til Health. Se gjennom innstillingen. Denne [veiledningen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) kan hjelpe deg med å forstå hvordan du konfigurerer varslingsinnstillingene for Azure AD Koble til tilstandsvarsler.
- Hvis du vil lære mer om AAD Koble til tilstandssynkroniseringsrapporten og hvordan du laster den ned, kan du se Rapport om synkronisering [på objektnivå](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Hvis du vil feilsøke AAD Koble til-tilstandsvarsler, følger du feilsøkingsveiledningen [for AAD Koble til](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) tilstandsvarsler om tilstandsdata og for vanlige spørsmål, kan du se Vanlige spørsmål om installasjon av [AAD Koble til Tilstand](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
