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
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004163"
---
# <a name="duplicate-device-record-in-the-portal"></a>Duplisert enhetspost i portalen

Det kan hende du ser to oppføringer for en enhet i portalen hvis enheten ikke rapporterer riktig delt administrasjonsstatus til nettstedet for konfigurasjonsbehandling. Hvis du vil kontrollere statusen for en enhet, kan du se gjennom **delt administrasjon**-kolonnen for enheten i konfigurasjonsbehandling-konsollen. Hvis kolonnen ikke vises, kan du legge den til ved å høyreklikke på en av kolonneoverskriftene og velge den fra listen.

Den verdien Delt administrasjon må være **Ja**. Hvis verdien er **Nei**, åpner du klient-appleten for konfigurasjonsbehandling på klientenheten og merker av for **Delt administrasjon**-egenskapen i Generelt-fanen.

- Hvis verdien er **Aktivert**, indikerer dette problemer med klientkommunikasjon ved administrasjonspunktet. Se gjennom **CcmMessaging.log** på enheten for å undersøke mulige tilkoblingsproblemer.

- Hvis verdien er **Deaktivert**, og enheten er registrert i Intune, må du kontrollere at enheten har mottatt policyen for delt administrasjon ved å gå gjennom **CoManagementHandler.log** på enheten.
