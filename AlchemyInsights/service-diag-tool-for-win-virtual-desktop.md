---
title: Tjeneste diagnose verktøy for Windows virtuelt skrive bord
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680238"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Tjeneste diagnose verktøy for Windows virtuelt skrive bord

Windows Virtual Desktop (WVD) har et diagnose verktøy som lar administratorer identifisere feil via ett enkelt grensesnitt. Dette verktøyet logger diagnose relatert informasjon når WVD brukes av noen som er tilordnet en WVD-rolle. Hver Logg inneholder informasjon om WVD-rollen som er involvert i aktiviteten, feil meldingene som vises under økten og informasjon om leieren og brukeren. Azure log Analytics kan konfigureres til å registrere aktivitets loggen som er opprettet av diagnose verktøyet. Slik gjør du det:

1. Opprett et Logg analyse arbeidsom råde med [Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2129500) eller [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Koble Windows-datamaskiner til Azure-skjerm](https://go.microsoft.com/fwlink/?linkid=2129913). Få arbeidsområde-ID-en og primær nøkkelen for arbeidsom rådet. Installasjons vei viseren trenger denne informasjonen for å konfigurere agenten på riktig måte og sikre at den kan kommunisere med Azure-skjermen.
1. [Push diagnose data til arbeidsom rådet](https://go.microsoft.com/fwlink/?linkid=2128284). Du kan skyve diagnose data fra WVD-leieren til Logg analysen for arbeidsom rådet.
1. [Identifisere og diagnostisere problemer](https://go.microsoft.com/fwlink/?linkid=2128338) som er interne eller eksterne i forhold til WVD.

Hvis du vil ha mer informasjon om hvordan du konfigurerer tjeneste diagnose verktøyet for WVD, kan du se [bruke Logg analyse for diagnose funksjonen](https://go.microsoft.com/fwlink/?linkid=2128084).
