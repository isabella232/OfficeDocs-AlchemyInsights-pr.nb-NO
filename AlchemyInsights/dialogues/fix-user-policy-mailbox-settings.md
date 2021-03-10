---
title: Løse brukerpolicy-/postboksinnstillinger
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695907"
---
# <a name="fix-user-policymailbox-settings"></a>Løse brukerpolicy-/postboksinnstillinger

Innstillingene for søppelpost i postboksen påvirket denne meldingen. Hvis du vil se gjennom innstillingene, gjør du følgende:

1. Start Skall for administrasjon av Exchange. Hvis du vil ha mer informasjon, [kan du se Åpne Exchange Management Shell.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Kjør denne kommandoen (ved hjelp av brukerens  **e-postadresse): get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Kontroller om avsenderens e-postadresse er en del av **TrustedSendersAndDomains** eller **BlockedSendersAndDomains.** Hvis e-postadressen er i en av listene, må du kanskje fjerne den. Hvis du vil ha mer informasjon, kan du se [Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
