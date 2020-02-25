---
title: Active Directory synkroniseres ikke
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265265"
---
# <a name="active-directory-not-syncing"></a>Active Directory synkroniseres ikke

Hvis du mottar synkroniseringsfeil, for eksempel "ingen nylig synkronisering", eller legg merke til katalogsynkroniseringsstatusen i Office-administratorportalen sier: "Sist synkronisert for mer enn 3 dager siden," kan det være at AADConnect har feil innstillinger eller utilstrekkelig tillatelser til å utføre en synkronisering.  

Hvis du installerer AADConnect på nytt ved hjelp av hurtiginnstillinger, kan du løse problemet raskt:

1. [Last ned den nyeste versjonen av AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Følg instruksjonene for uttrykkelig installasjon](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Hvis du vil ha mer informasjon om AADConnect-tjenestekontoer, kan du se [Azure AD Connect: Kontoer og tillatelser](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
