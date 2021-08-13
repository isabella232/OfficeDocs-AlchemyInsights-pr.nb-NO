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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937110"
---
# <a name="active-directory-not-syncing"></a>Active Directory synkroniseres ikke

Hvis du mottar synkroniseringsfeil, for eksempel «ingen nylig synkronisering», eller legger merke til katalogsynkroniseringsstatusen i Office-administrasjonsportalen, sier «Sist synkronisert for mer enn 3 dager siden», kan det være at AADConnect har feil innstillinger eller utilstrekkelige tillatelser til å utføre en synkronisering.  

Hvis du installerer AADConnect på nytt ved hjelp av hurtiginnstillinger, kan problemet løses raskt:

1. [Last ned den nyeste versjonen av AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Følg instruksjonene for ekspressinstallasjon](/azure/active-directory/hybrid/how-to-connect-install-express).

Azure AD Connect må installeres på Windows-2012 eller nyere. Denne serveren må være domene-tilkoblet og være en domenekontroller eller en medlemsserver. Hvis du vil ha en fullstendig liste over Azure AD Koble til krav og forhåndskrav, kan du se gjennom Forutsetninger [for Azure AD Koble til.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Hvis du vil ha mer informasjon om AADConnect-tjenestekontoer, [kan du se Azure AD Koble til: Kontoer og tillatelser](/azure/active-directory/hybrid/reference-connect-accounts-permissions).
