---
title: Får ikke tilgang til fellesmapper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959503"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan ikke koble til fellesmapper

Hvis fellesmappe tilgang ikke fungerer for noen brukere, kan du prøve følgende:

Koble til EXO PowerShell, og Konfigurer DefaultPublicFolderMailbox på problem brukerkontoen slik at den samsvarer med en på en brukerkonto som fungerer.

Eksempel:

Get-postboks WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Sett postboks ProblemUser-DefaultPublicFolderMailbox \<verdi fra forrige kommando>

Vent minst en time for at endringen skal tre i kraft.