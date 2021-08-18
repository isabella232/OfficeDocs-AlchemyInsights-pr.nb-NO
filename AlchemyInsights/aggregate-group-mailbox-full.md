---
title: AggregateGroupMailbox full NDR mottatt for e-post sendt til Microsoft 365 gruppe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315919"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox full NDR mottatt for e-post sendt til Microsoft 365 gruppe

Bruk følgende EXO-skallkommando til å opprette en Exchange transportregel for å slippe e-postmeldinger som sendes til aggregert gruppepostboks:

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**Obs!** Erstatt SMTP-adressen i **-SentTo** med SMTP-adressen til samlet gruppepostboks i leieren. Du kan få SMTP-adressen til samlet gruppepostboks fra NDR-en som mottas.



