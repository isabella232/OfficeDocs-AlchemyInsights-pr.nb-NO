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
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030911"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Diagnostikk for ulike tilgangsproblemer for porter

Gjør følgende for å løse de ulike porttilgangsproblemene:

1. Stopp/deallocate the virtual machine (VM) from the portal, restart the VM, and test again. 
2. Kontroller nettverksinnstillingene for VM for å finne ut om du har nettverkssikkerhetsgrupper (NSGs) som blokkerer trafikk. Du kan også bruke Kontrollverktøy for IP-flyt i [Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) til å se etter NSGs som blokkerer trafikk, User-Defined Routes (UDRs) omdirigere trafikken tilbake til lokalt (Standardrute' 0.0.0.0/0) eller til et nettverksutstyr.
Hvis du fremdeles opplever problemer etter at du har prøvd fremgangsmåten ovenfor, kan du angi VM-navnet og TCP-porten du prøver å sende e-post på for ytterligere diagnose.

**Anbefalte dokumenter**

[Begrensninger og anbefalinger for sending av utgående e-post over port 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)