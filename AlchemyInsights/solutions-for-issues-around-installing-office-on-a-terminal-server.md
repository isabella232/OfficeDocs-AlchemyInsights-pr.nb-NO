---
title: Løsninger for problemer rundt installasjon av office på en Terminal Server
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: cc2d2b1a5c73e729a67b1e6f36fdcff2125541ca
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010911"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a>Løsninger for problemer rundt installasjon av office på en Terminal Server

Hvis du vil bruke aktivisering av delt datamaskin, må du ha et abonnement som inkluderer Microsoft 365 Apps for enterprise.
  
- Kontroller at aktivering av delt datamaskin er aktivert
- Kontroller at aktiveringen var vellykket
- Se gjennom feilmeldinger for delt datamaskinaktivering:
- "Produktene vi fant i kontoen din, kan ikke brukes til å aktivere Office i scenarier for delte datamaskiner"
  
Denne feilen betyr at du ikke har et abonnement som inkluderer Microsoft 365 Apps for enterprise.

"Ulisensiert produkt"

- Kontroller at brukeren er tilordnet en lisens for Microsoft 365 Apps for enterprise.
- Kontroller at brukeren logger på med brukerkontoen sin.
- Kontroller at det er tilkobling mellom den delte datamaskinen og Internett.

Hvis du vil ha andre tips om feilsøking, kan du [se: Feilsøke problemer med delt datamaskinaktivering](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)