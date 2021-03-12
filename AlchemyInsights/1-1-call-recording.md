---
title: 1:1 samtaleopptak
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
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733858"
---
# <a name="11-call-recording"></a>1:1 samtaleopptak

Administratorer må nå gjøre noe for å fortsette å tillate brukere å spille inn 1:1-anrop.
 
Fra og med 12. april 2021 begynner vi å bruke et nytt alternativ for anropspolicy for Teams *AllowCloudRecordingForCalls.* 

Funksjonene for samtaleinnspilling 1:1 kontrolleres for øyeblikket av *tillatCloudRecording-alternativet* i teams møtepolicyer. Hvis brukerne har tillatelse til å spille inn Teams-møter, kan de også ta opp 1:1-samtaler.

Hvis du foretrekker å blokkere alle brukere fra å spille inn 1:1-samtaler, trenger du ikke å gjøre noe. *AllowCloudRecordingForCalls* anropspolicyalternativ velges $False som standard.

Denne endringen er dokumentert i følgende meldingssenterinnlegg: (oppdatert) innføring i policy for innspilling av anrop [1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) For å angi alternativet for anropspolicy for Teams, må du bruke [Teams PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)

**Slik aktiverer du samtaleopptak i 1:1-samtaler:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True

**Slik deaktiverer du samtaleopptak i 1:1-samtaler:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False

