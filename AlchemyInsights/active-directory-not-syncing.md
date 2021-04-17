---
title: Active Directory synkroniseres ikke
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822860"
---
# <a name="active-directory-not-syncing"></a>Active Directory synkroniseres ikke

Hvis du mottar synkroniseringsfeil, for eksempel «ingen nylig synkronisering», eller legger merke til at statusen for katalogsynkronisering i administrasjonsportalen for Office sier «Sist synkronisert for mer enn 3 dager siden», kan det være at AADConnect har feil innstillinger eller utilstrekkelige tillatelser til å utføre en synkronisering.  

Hvis du installerer AADConnect på nytt ved hjelp av hurtiginnstillinger, kan dette løse problemet raskt:

1. [Last ned den nyeste versjonen av AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Følg instruksjonene for ekspressinstallasjon](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Hvis du vil ha mer informasjon om AADConnect-tjenestekontoer, kan du se [Azure AD Connect: Kontoer og tillatelser](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
