---
title: Duplisert enhetspost i portalen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814525"
---
# <a name="duplicate-device-record-in-the-portal"></a>Duplisert enhetspost i portalen

Det kan hende du ser to oppføringer for en enhet i portalen hvis enheten ikke rapporterer riktig delt administrasjonsstatus til nettstedet for konfigurasjonsbehandling. Hvis du vil kontrollere statusen for en enhet, kan du se gjennom **delt administrasjon**-kolonnen for enheten i konfigurasjonsbehandling-konsollen. Hvis kolonnen ikke vises, kan du legge den til ved å høyreklikke på en av kolonneoverskriftene og velge den fra listen.

Den verdien Delt administrasjon må være **Ja**. Hvis verdien er **Nei**, åpner du klient-appleten for konfigurasjonsbehandling på klientenheten og merker av for **Delt administrasjon**-egenskapen i Generelt-fanen.

- Hvis verdien er **Aktivert**, indikerer dette problemer med klientkommunikasjon ved administrasjonspunktet. Se gjennom **CcmMessaging.log** på enheten for å undersøke mulige tilkoblingsproblemer.

- Hvis verdien er **Deaktivert**, og enheten er registrert i Intune, må du kontrollere at enheten har mottatt policyen for delt administrasjon ved å gå gjennom **CoManagementHandler.log** på enheten.
