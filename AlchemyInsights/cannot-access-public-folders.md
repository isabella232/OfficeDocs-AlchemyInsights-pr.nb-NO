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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891758"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook kan ikke koble til fellesmapper

Hvis fellesmappetilgang ikke fungerer for noen brukere, kan du prøve følgende:

Koble til EXO PowerShell og konfigurer parameteren DefaultPublicFolderMailbox på problembrukerkontoen slik at den samsvarer med parameteren på en fungerende brukerkonto.

Eksempel:

Get-Postboks WorkingUser | ft DefaultPublicFolderMailbox, EffektivFellesMappeKasse

Set-postboks ProblemUser -DefaultPublicFolderMailbox-verdien \<fra forrige kommando>

Vent minst en time på at endringen trer i kraft.

Hvis problemet forblir, følger du [denne fremgangsmåten](https://aka.ms/pfcte) for å feilsøke tilgangsproblemer for fellesmapper ved hjelp av Outlook.