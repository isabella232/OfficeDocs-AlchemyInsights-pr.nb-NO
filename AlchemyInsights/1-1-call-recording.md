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
ms.openlocfilehash: c17408442cec6c0877b7d66bc8a7fd3062eb0e47
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314393"
---
# <a name="11-call-recording"></a>1:1 samtaleopptak

Hvis **Start innspilling-knappen** er nedtonet i et 1:1-anrop, må du endre policyinnstillingene for den berørte brukeren. Hvis du vil kontrollere policyinnstillingen, kjører du Diagnose for den berørte brukeren ved å skrive **inn Diag: Teams 1:1 Samtaleinnspilling** ovenfor.     

Fra og med 31. mai 2021 begynner vi å bruke en ny Teams Policy for anrop *AllowCloudRecordingForCalls*. Før denne endringen kontrolleres 1:1-samtaleinnspillingen av *AllowCloudRecording* Teams møtepolicyen. Denne endringen er dokumentert i meldingssenterinnlegget: [(Oppdatert) 01:01](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)Innføring i policy for innspilling av anrop .  

*AllowCloudRecordingForCalls*   alternativet for anropspolicy er satt **til $False** som standard. Hvis du foretrekker å blokkere alle brukere fra å spille inn 1:1-anrop, trenger du ikke å gjøre noe.  

Hvis du vil aktivere anropsopptak for alle brukere i 1:1-anrop, bruker [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) til å kjøre følgende cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Du kan også opprette en ny policy og angi **-AllowCloudRecordingForCalls** til $true og tilordne denne policyen til brukerne.  

Hvis du vil ha mer informasjon, kan [du se 1:1 Policykontroller for innspilling av anrop er (nesten!) Her](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
