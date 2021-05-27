---
title: Programvarelager mangler eller er unøyaktig
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676509"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>Programvarelager mangler eller er unøyaktig

Programvarebeholdningen i Håndtering av trusler og sikkerhetsproblemer (TVM) er en liste over kjent programvare i organisasjonen med offisielle Common Platform Enumerations (CPE).

Programvareprodukter uten en offisiell CPE har ikke publisert sikkerhetsproblemer. Beholdningen inneholder også detaljer som navnet på leverandøren, antall svakheter, trusler og antall eksponerte enheter.

Programvareendringer på enheter gjenspeiles vanligvis i sikkerhetsportaler innen to timer. Det kan imidlertid noen ganger ta lengre tid. Det er for øyeblikket ikke mulig å fremtvinge en synkronisering. dette er en kontinuerlig vurdering.

Hvis du har gjort en programvareendring og endringen ikke gjenspeiles nøyaktig i TVM etter fem timer, følger du disse trinnene:

1. Se delen om programvarebevis for å forstå hvordan programvaren ble oppdaget.
1. Kontroller at programvaren støttes. Programvaren kan bare være synlig på enhetsnivå selv om den for øyeblikket ikke støttes av Håndtering av trusler og sikkerhetsproblemer. Men bare begrensede data er tilgjengelig.
1. Hvis du vil se fremgangsmåten for å rapportere unøyaktighet fra portalen, kan du se [Rapportere unøyaktighet](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).
   
    **Obs!** Rapportering av unøyaktighet fra MDE-portalen er en enveis kanal til ingeniørarbeid. Hvis problemet haster, åpner du en støtteforespørsel.

Hvis du vil ha mer informasjon, kan [du se Programvarebeholdning – Håndtering av trusler og sikkerhetsproblemer](/microsoft-365/security/defender-endpoint/tvm-software-inventory).