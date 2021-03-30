---
title: Single-Sign på for Azure Active Directory-sammenføyde enheter
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405051"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a>Enkel pålogging for Azure Active Directory-sammenføyde enheter

Hvis du har et lokalt Active Directory-miljø (AD)-miljø og vil bli med i AD-domeneaktiverte datamaskiner til Azure AD, kan du oppnå dette ved å gjøre hybrid Azure AD-sammenføyning. [Slik gjør du det: Planlegg implementeringen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) av hybrid Azure Active Directory-sammenføyning gir deg de relaterte trinnene for å implementere en hybrid Azure AD-sammenføyning i miljøet.

[Konfigurere Azure AD-sammenføyde enheter for lokale Single-Sign På ved hjelp av Windows Hello for Business](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

**Problemer med primær oppdateringstoken (PRT)** Et primært oppdateringstoken (PRT) er en viktig artefakt av Azure AD-godkjenning på Windows 10-, Windows Server 2016- og nyere versjoner, iOS- og Android-enheter. Det er et JSON Web Token (JWT) spesielt utstedt til Microsofts førsteparts tokenmeglere for å aktivere enkel pålogging (SSO) på tvers av programmene som brukes på disse enhetene. [I Hva er et primært oppdateringstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)gir vi detaljer om hvordan en PRT utstedes, brukes og beskyttes på Windows 10-enheter.

**WamDefaultSet: JA og AzureADPrt: JA** Disse feltene angir om brukeren har godkjent Azure AD ved pålogging på enheten. Hvis verdiene er **NEI,** kan det forfalle:

- Ugyldig lagringsnøkkel i TPM som er knyttet til enheten ved registrering (kontroller KeySignTest mens den kjører forhøyet).
- Alternativ påloggings-ID
- Finner ikke HTTP-proxy

Feilsøke enheter ved hjelp av kommandoen dsregcmd – [SSO-tilstand](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)
