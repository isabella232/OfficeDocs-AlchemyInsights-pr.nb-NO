---
title: Konfigurere MIM-synkroniseringstjenesten
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481869"
---
# <a name="configure-mim-sync-service"></a>Konfigurere MIM-synkroniseringstjenesten

Synkroniseringstjenesten for Microsoft Identity Manager (MIM) er en komponent i MIM. Det er en sentralisert lokal tjeneste som lagrer og integrerer informasjon for organisasjoner som har flere lokale kataloger og databaser. Du kan kanskje løse problemet med MIM-synkronisering hvis problemet ble løst i en nylig oppdatering til MIM eller er et av de andre problemene som nevnes i avsnittet nedenfor.

**Anbefalte trinn**

1. Kontroller at du bruker en nylig oppdatering av MIM-synkronisering, og se produktmerknene for [MIM-synkronisering](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) for å finne ut om problemet er løst i en oppdatering.
2. Hvis problemet ligger i koblingene Generic LDAP, Generic SQL, Lotus Domino eller Web Services, må du kontrollere at du bruker en nylig oppdatering av de [generiske koblingene.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)
3. Hvis en MIM-synkroniseringskjøring stopper med en [](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) feil, kan du se i feiltabellen for å finne potensielle årsaker.
4. Hvis kjøringen stopper med **extension-dll-exception,** klikker du på disse ordene for å åpne vinduet for egenskaper for koblingsområdeobjektet, og klikker på **Stack Trace...** for å se mer informasjon om den underliggende årsaken, som beskrevet i [Extension-DLL-Exception.](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx) 
5. Hvis PCNS-komponenten (Password Change Notification Service) rapporterer feil **6025** i hendelsesloggen under passordsynkronisering, kan du se i veiledningen for feilsøking av [PCNS-rapportfeil 6025.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)
6. Hvis full synkronisering med FIM Service Management  Agent er treg, kontrollerer du innstillingen for automatisk vekst for TempDB, som beskrevet i Feilsøking av treg eller [hengende full synkronisering.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)
7. Hvis det oppstår en feil med server som har blitt stoppet, med mislykket oppretting via nettjenester ved hjelp av FIM Service Management Agent, kan du se [Støtteinformasjon: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for å få en oversikt over årsaker.

