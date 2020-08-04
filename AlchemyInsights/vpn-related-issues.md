---
title: VPN-relaterte problemer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555232"
---
# <a name="vpn-related-issues"></a>VPN-relaterte problemer

Vellykket implementering av VPN-tilkobling for MDM-klienter avhenger av en distribuert profil som gjenspeiler kravene til VPN-infrastrukturen på riktig måte. Hvis du vil ha de riktige innstillingene for klientplattformene du undersøker, kan du se: 

[Windows 10 og Windows Holografiske enhetsinnstillinger for å legge til VPN-tilkoblinger ved hjelp av Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Legge til VPN-innstillinger på iOS- og iPadOS-enheter i Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Innstillinger for Android-enheter for å konfigurere VPN i Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Legge til VPN-innstillinger på macOS-enheter i Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Hvis VPN-profilen din bruker sertifikatbasert godkjenning, må du kontrollere at rotsertifikat- og klientgodkjenningssertifikatprofilene som er koblet til VPN-profilen, distribueres.

**Vanlige problemer**

**Jeg distribuerte en VPN-profil til en enhet. Intune viser at det var vellykket, men enheten kobler ikke til VPN.**

En vellykket status betyr at Intune har distribuert profilen som konfigurert. Disse konfigurasjonene samsvarer imidlertid kanskje ikke med kravene til nettverket og/eller godkjenningen. Se gjennom logger i infrastruktur- og godkjenningstjenesten (på VPN-serveren og NPS/Radius-serveren) hvis du vil ha mer informasjon om den forsøkte tilkoblingen. Du må kanskje samarbeide med nettverksinfrastrukturteamet ditt, eller tredjeparts VPN-leverandøren, for å samle inn og gjennomgå logger.

**Når jeg konfigurerer et egendefinert VPN for iOS, er ikke VPN-funksjonen per app gjort tilgjengelig.**

VPN per app for iOS-enheter i Intune er for øyeblikket tilgjengelig for en bestemt liste over leverandører og partnere, som også må oppfylle sertifikatforutsetninger før du konfigurerer et VPN per app. Hvis du vil ha mer informasjon, kan du se [Konfigurere VPN (Virtual Private Network) per app for iOS/iPadOS-enheter i Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Hvis du vil ha mer informasjon om alle VPN-tilkoblingstyper i Intune, kan du se [Opprette VPN-profiler for å koble til VPN-servere i Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**iOS On-Demand VPN utløses ikke når et konfigurert domene er tilgjengelig**

Hvis du vil teste automatiske VPN-innstillinger, angir du følgende verdier:

Jeg vil gjøre følgende: **Evaluere hvert tilkoblingsforsøk** 

Velg om du vil koble til: **Koble til om nødvendig**

Når brukere får tilgang til disse domenene: **mål** *domenenavn*

Hvis konfigurasjonen ovenfor ikke er vellykket, legger du til følgende element:

Når denne URL-adressen ikke kan nås, kan du koble til VPN: **BADURL**