---
title: Diagnostikk for ulike tilgangsproblemer for porter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035778"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostikk for ulike tilgangsproblemer for porter

Gjør følgende for å løse de ulike porttilgangsproblemene:

1. Stopp/deallocate the virtual machine (VM) from the portal, restart the VM, and test again. 
2. Kontroller nettverksinnstillingene for VM for å finne ut om du har nettverkssikkerhetsgrupper (NSGs) som blokkerer trafikk. Du kan også bruke Kontrollverktøy for IP-flyt i [Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) til å se etter NSGs som blokkerer trafikk, User-Defined Routes (UDRs) omdirigere trafikken tilbake til lokalt (Standardrute' 0.0.0.0/0) eller til et nettverksutstyr.
Hvis du fremdeles opplever problemer etter at du har prøvd fremgangsmåten ovenfor, kan du angi VM-navnet og TCP-porten du prøver å sende e-post på for ytterligere diagnose.

**Anbefalte dokumenter**

[Begrensninger og anbefalinger for sending av utgående e-post over port 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)