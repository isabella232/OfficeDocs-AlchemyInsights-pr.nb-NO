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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696967"
---
# <a name="11-call-recording"></a>1:1 samtaleopptak

Hvis **Start innspilling-knappen** er nedtonet i et 1:1-anrop, må du endre policyinnstillingene for den berørte brukeren.   

Fra og med 31. mai 2021 begynner vi å bruke en ny Teams Policy for anrop *AllowCloudRecordingForCalls*. Før denne endringen kontrolleres 1:1-samtaleinnspillingen av *AllowCloudRecording* Teams møtepolicyen. Denne endringen er dokumentert i meldingssenterinnlegget: [(Oppdatert) 01:01](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)Innføring i policy for innspilling av anrop .  

*AllowCloudRecordingForCalls*   alternativet for anropspolicy er satt **til $False** som standard. Hvis du foretrekker å blokkere alle brukere fra å spille inn 1:1-anrop, trenger du ikke å gjøre noe.  

Hvis du vil aktivere samtaleopptak for alle brukere i 1:1-anrop, bruker Teams PowerShell til å kjøre følgende cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Du kan også opprette en ny policy og angi **-AllowCloudRecordingForCalls** til å $true og tilordne denne policyen til brukerne.  

Hvis du vil ha mer informasjon, kan [du se 1:1 Policykontroller for innspilling av anrop er (nesten!) Her](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
