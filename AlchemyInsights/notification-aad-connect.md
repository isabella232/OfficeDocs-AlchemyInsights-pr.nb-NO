---
title: Varsel AAD Koble til
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
- "9003245"
- "9326"
ms.openlocfilehash: b8713700ee4fc8863a269c99b92954e1df45e1e647c491fb9b439ab83c49f2ff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097315"
---
# <a name="notification-aad-connect"></a>Varsel AAD Koble til

- Kontroller at du er autorisert til å utføre operasjonen. Globale administratorer har tilgang som standard. I tillegg kan du bruke rollebasert [tilgangskontroll til](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) å delegere registreringstillatelse til bidragsyter.
- Kontroller at de nødvendige endepunktene er aktivert, og ikke blokkert på grunn av brannmuren. Hvis du vil ha mer informasjon, kan du se [krav](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registreringen kan mislykkes på grunn av at utgående kommunikasjon blir utsatt for SSL-inspeksjon av nettverkslaget.
- Kontroller at du har bekreftet varslingsinnstillingene for Azure AD Koble til Health, og se gjennom innstillingen. Hvis du vil forstå hvordan du konfigurerer varslingsinnstillingene for Azure AD Koble til tilstandsvarsler, kan du se denne [veiledningen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Hvis du vil lære mer om AAD Koble til tilstandssynkroniseringsrapporten og hvordan du laster den ned, kan du se Rapport om synkronisering [på objektnivå](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Hvis du vil feilsøke AAD Koble til-tilstandsvarsler, følger du feilsøkingsveiledningen [for AAD Koble til](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) tilstandsvarsler og vanlige spørsmål ved å se Vanlige spørsmål om [AAD-Koble til tilstandsinstallasjon](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
