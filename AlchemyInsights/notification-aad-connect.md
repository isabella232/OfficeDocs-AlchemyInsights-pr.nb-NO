---
title: Varsel AAD Connect
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
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036106"
---
# <a name="notification-aad-connect"></a>Varsel AAD Connect

- Kontroller at du er autorisert til å utføre operasjonen. Globale administratorer har tilgang som standard. I tillegg kan du bruke rollebasert [tilgangskontroll til](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) å delegere registreringstillatelse til bidragsyter.
- Kontroller at de nødvendige endepunktene er aktivert, og ikke blokkert på grunn av brannmuren. Hvis du vil ha mer informasjon, kan du se [krav](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Registreringen kan mislykkes på grunn av at utgående kommunikasjon blir utsatt for SSL-inspeksjon av nettverkslaget.
- Kontroller at du har bekreftet varslingsinnstillingene for Azure AD Connect Health og se gjennom innstillingen. Hvis du vil forstå hvordan du konfigurerer varslingsinnstillingene for Azure AD Connect-tilstandsvarsler, kan du se denne [veiledningen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).
- Hvis du vil lære mer om rapporten om AAD Connect Health-synkronisering og hvordan du laster den ned, kan du se Rapport om synkronisering [på objektnivå](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Hvis du vil feilsøke tilstandsvarsler for AAD Connect, følger du feilsøkingsveiledningen for AAD Connect Health [data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see Common [AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).
