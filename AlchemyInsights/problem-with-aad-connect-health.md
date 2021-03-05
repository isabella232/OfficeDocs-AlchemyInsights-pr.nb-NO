---
title: Problem med AAD Connect Health
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
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482072"
---
# <a name="problem-with-aad-connect-health"></a>Problem med AAD Connect Health

- Kontroller at du er autorisert til å utføre operasjonen. Globale administratorer har tilgang som standard. I tillegg kan du bruke [rollebasert](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) tilgangskontroll til å delegere registreringstillatelse til Bidragsyter.
- Sikre at de nødvendige endepunktene er aktivert, og at de ikke blokkeres på grunn av brannmuren. Hvis du vil ha mer informasjon, kan du [se krav.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Registrering kan mislykkes på grunn av at utgående kommunikasjon er underlagt SSL-inspeksjon av nettverkslaget.
- Kontroller at du har bekreftet varslingsinnstillingene for Azure AD Connect Health. Se gjennom innstillingen. Denne [veiledningen](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) kan hjelpe deg med å forstå hvordan du konfigurerer varslingsinnstillingene for azure AD Connect-tilstandsvarsler.
- Hvis du vil lære mer om rapporten om AAD Connect-tilstandssynkronisering og hvordan du laster den ned, kan du se [synkroniseringsrapport på objektnivå.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Hvis du vil feilsøke tilstandsvarsler for AAD Connect, kan du følge feilsøkingsveiledningen for varsler om tilstandsoppdretting for [AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Health og se vanlige spørsmål om [AAD Connect Health-installasjon.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
