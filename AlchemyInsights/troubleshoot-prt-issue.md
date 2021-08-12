---
title: Feilsøke PRT-problem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972725"
---
# <a name="troubleshoot-prt-issue"></a>Feilsøke PRT-problem

For at en enhet skal kunne fullføre godkjenningen, må den være fullstendig registrert og i god stand og kunne skaffe et primært oppdateringstoken (PRT).

Registreringsprosessen for hybrid Azure AD-sammenføyning krever at enhetene er på et bedriftsnettverk. Det fungerer også over VPN, men det finnes noen begrensninger for dette. Vi har hørt at kunder trenger hjelp med feilsøking av registreringsprosessen for hybrid Azure AD-bli med under eksterne arbeidsforhold. Her er en oversikt over hva som skjer under panseret under registreringsprosessen.

**Skygodkjenningsmiljø (ved hjelp av Hash-synkronisering av passord for Azure AD eller gjennomgangsgodkjenning)**

Denne registreringsflyten kalles også «Synkroniser sammenføyning».

1. Windows 10 oppdager en SCP-post når brukeren logger på enheten.
    1. Enheten prøver først å hente leierinformasjon fra klientsidens SCP i registeret [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Hvis den mislykkes, kommuniserer enheten med lokal Active Directory (AD) for å få leierinformasjon fra Service Connection Point (SCP). Hvis du vil bekrefte SCP, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Vi anbefaler at du aktiverer SCP i AD og bare bruker SCP på klientsiden for første validering.

2. Windows 10 prøver å kommunisere med Azure AD under systemkonteksten for å godkjenne seg selv mot Azure AD. Du kan kontrollere om enheten har tilgang til Microsoft-ressurser under systemkontoen ved hjelp av skriptet Test tilkobling for enhetsregistrering.

3. Windows 10 genererer et selvsignert sertifikat og lagrer det under datamaskinobjektet i lokal AD. Dette krever domenekontrollerens linje for synslinje.

4. Et enhetsobjekt som har et sertifikat, synkroniseres til Azure AD via Azure AD Koble til. Synkroniseringssyklusen er som standard hvert 30. minutt, men det avhenger av konfigurasjonen av Azure AD Koble til. Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. På dette stadiet skal du kunne se emneenheten i Ventende tilstand under Enhetsblad i Azure Portal.

6. Ved neste brukerpålogging Windows 10, fullføres registreringen. 

> [!NOTE]
> Hvis du bruker VPN og en avloggingsprosess avslutter domenetilkoblingen, kan du utløse registrering manuelt:
 1. Problem a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC. PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Hvis du vil ha mer informasjon om problemer med hybrid sammenføyning, kan du [se Feilsøke problemer med enheter](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
