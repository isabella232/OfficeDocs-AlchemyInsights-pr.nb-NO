---
title: Tjenestediagnoseverktøy for Windows virtuelt skrivebord
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
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052395"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Tjenestediagnoseverktøy for Windows virtuelt skrivebord

Windows Virtual Desktop (WVD) tilbyr et diagnoseverktøy som lar administratorer identifisere feil via ett enkelt grensesnitt. Dette verktøyet logger diagnoserelatert informasjon når WVD brukes av noen som har tilordnet en WVD-rolle. Hver logg inneholder informasjon om WVD-rollen som er involvert i aktiviteten, feilmeldingene som vises under økten, og informasjonen om leieren og brukeren. Azure Log Analytics kan konfigureres til å registrere aktivitetsloggen som er opprettet av diagnoseverktøyet. Slik gjør du det:

1. Opprett et Log Analytics-arbeidsområde med [Azure-portalen](https://go.microsoft.com/fwlink/?linkid=2129500) [eller Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Koble til Windows datamaskiner til Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Få arbeidsområde-ID-en og primærnøkkelen for arbeidsområdet. Konfigurasjonsveiviseren trenger denne informasjonen for å konfigurere agenten på riktig måte, og for å sikre at den kan kommunisere med Azure Monitor.
1. [Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284). Du kan flytte diagnosedata fra WVD-leieren til Logganalyse for arbeidsområdet.
1. [Identifiser og diagnostiser problemer](https://go.microsoft.com/fwlink/?linkid=2128338) som er interne eller eksterne i forhold til WVD.

Hvis du vil lære mer om hvordan du konfigurerer diagnoseverktøyet for tjenesten for WVD, kan du se Bruke [Logganalyse for diagnosefunksjonen](https://go.microsoft.com/fwlink/?linkid=2128084).
