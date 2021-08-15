---
title: Feilsøke enkel pålogging for Azure AD-sammenføyde enheter
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: 872333e13bb51b3a22431154627ad561f6db88c681c9eeee523fdd09e58c0371
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54039255"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a>Feilsøke enkel pålogging for Azure AD-sammenføyde enheter

Hvis du har et lokalt Active Directory-miljø (AD)-miljø og vil bli med i AD-domeneaktiverte datamaskiner til Azure AD, kan du oppnå dette ved å gjøre hybrid Azure AD-sammenføyning. [Slik planlegger du hybrid-Azure Active Directory-implementeringen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) gir deg de relaterte trinnene for å implementere en hybrid Azure AD-sammenføyning i miljøet.

Hvis du vil ha mer informasjon, kan du se [Konfigurere Azure AD-sammenføyde](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)enheter for lokale Single-Sign På ved hjelp av Windows Hello for Business .

**Problemer med primær oppdateringstoken (PRT)**

Et primært oppdateringstoken (PRT) er en viktig artefakt av Azure AD-godkjenning på Windows 10-, Windows Server 2016- og nyere versjoner, iOS- og Android-enheter. Det er et JSON Web Token (JWT) spesielt utstedt til Microsofts førsteparts tokenmeglere for å aktivere enkel pålogging (SSO) på tvers av programmene som brukes på disse enhetene. Hvis du vil ha mer informasjon om hvordan en PRT utstedes, brukes og beskyttes på Windows 10 enheter, kan du se Hva er et [primært oppdateringstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

**WamDefaultSet: JA og AzureADPrt: JA**

Disse feltene angir om brukeren har godkjent Azure AD ved pålogging på enheten. Hvis verdiene er **NEI,** kan det skyldes følgende:

- Ugyldig lagringsnøkkel i TPM som er knyttet til enheten ved registrering (kontroller KeySignTest mens den kjører forhøyet)
- Alternativ påloggings-ID
- Finner ikke HTTP-proxy

Hvis du vil feilsøke enheter ved hjelp av dsregcmd-kommandoen, kan du [se SSO-tilstand](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).
