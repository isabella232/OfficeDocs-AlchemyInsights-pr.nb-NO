---
title: Tjenestediagnoseverktøy for Windows Virtual Desktop
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595865"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Tjenestediagnoseverktøy for Windows Virtual Desktop

Windows Virtual Desktop (WVD) tilbyr et diagnoseverktøy som lar administratorer identifisere feil gjennom ett enkelt grensesnitt. Dette verktøyet logger diagnoserelatert informasjon når WVD brukes av noen som har tilordnet en WVD-rolle. Hver logg inneholder informasjon om WVD-rollen som er involvert i aktiviteten, feilmeldingene som vises under økten, og informasjonen om leieren og brukeren. Azure Log Analytics kan konfigureres til å registrere aktivitetsloggen som er opprettet av diagnoseverktøyet, ved å følge disse trinnene:

1. Opprett et Log Analytics-arbeidsområde med [Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2129500) eller [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Koble Windows-datamaskiner til Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Få arbeidsområde-ID-en og primærnøkkelen for arbeidsområdet. Konfigurasjonsveiviseren trenger denne informasjonen for å konfigurere agenten på riktig måte, og for å sikre at den kan kommunisere med Azure Monitor.

1. [Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284). Du kan flytte diagnosedata fra WVD-leieren til Logganalyse for arbeidsområdet.

1. [Identifiser og diagnostiser](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problemer som er interne eller eksterne i forhold til WVD.

Hvis du vil lære mer om hvordan du konfigurerer tjenestediagnoseverktøyet for WVD, kan du se Bruke Logganalyse for diagnosefunksjonen.