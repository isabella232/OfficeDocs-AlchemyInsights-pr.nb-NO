---
title: Løse innstillinger for brukerpolicy/postboks
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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034727"
---
# <a name="fix-user-policymailbox-settings"></a>Løse innstillinger for brukerpolicy/postboks

Innstillingene for søppelpost i postboksen påvirket denne meldingen. Gjør følgende for å se gjennom innstillingene:

1. Start Exchange administrasjonsskall. Hvis du vil ha mer informasjon, [kan du se Åpne Exchange Administrasjonsskall](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Kjør denne kommandoen (ved hjelp av brukerens  **e-postadresse): get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Kontroller om avsenderens e-postadresse er en del av **TrustedSendersAndDomains** eller **BlockedSendersAndDomains**. Hvis e-postadressen er i en av listene, må du kanskje fjerne den. Hvis du vil ha mer informasjon, [kan du se Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
