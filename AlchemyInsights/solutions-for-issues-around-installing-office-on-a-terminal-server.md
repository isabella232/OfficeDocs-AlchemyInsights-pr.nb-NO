---
title: Løsninger på problemer ved installasjon av Office på en Terminal Server
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: 28ebe2b1375b142ca63dc686c7afbbe88abfd539a93780cff3861f80de40b411
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021857"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a>Løsninger på problemer ved installasjon av Office på en Terminal Server

Hvis du vil bruke aktivering av delt datamaskin, må du ha et abonnement som inneholder Microsoft 365 Apps for enterprise.
  
- Kontroller at aktivering av delt datamaskin er aktivert
- Kontroller at aktiveringen var vellykket
- Se gjennom feilmeldinger for aktivering av delt datamaskin:
- «Produktene vi fant i kontoen din, kan ikke brukes til å aktivere Office i scenarioer for delte datamaskiner»
  
Denne feilen betyr at du ikke har et abonnement som inneholder Microsoft 365 Apps for enterprise.

«Ulisensiert produkt»

- Kontroller at brukeren er tilordnet en lisens for Microsoft 365 Apps for enterprise.
- Kontroller at brukeren logger på med brukerkontoen sin.
- Kontroller at det er tilkobling mellom den delte datamaskinen og Internett.

Hvis du vil ha andre feilsøkingstips, kan du se: [Feilsøke problemer med aktivering av delt datamaskin](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)