---
title: Active Directory ikke synkronisere
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697638"
---
# <a name="active-directory-not-syncing"></a>Active Directory ikke synkronisere

Hvis du får synkroniserings feil, for eksempel «ingen nylig synkronisering», eller Legg merke til at statusen for katalog synkronisering i Office Admin-portalen sier at «sist synkronisert for mer enn 3 dager siden», kan være at AADConnect har feil innstillinger eller utilstrekkelige tillatelser til å utføre en synkronisering.  

Å installere AADConnect på nytt ved hjelp av innstillingene for Express kan løse problemet raskt:

1. [Last ned den nyeste versjonen av AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Følg instruksjonene for hurtig installasjon](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Hvis du vil ha mer informasjon om AADConnect-tjeneste kontoer, kan du se [Azure ad Connect: kontoer og tillatelser](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
