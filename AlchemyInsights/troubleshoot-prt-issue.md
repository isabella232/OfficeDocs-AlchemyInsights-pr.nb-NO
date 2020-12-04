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
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573721"
---
# <a name="troubleshoot-prt-issue"></a>Feilsøke PRT-problem

For at alle enheter skal kunne bli godkjent, må den være fullstendig registrert og i god tilstand og ha mulighet til å skaffe seg et primært PRT (Primary Fresh token).

Hybrid registrerings prosessen for Azure AD JOIN krever at enheter er på et bedrifts nettverk. Det fungerer også over VPN, men det er noen advarsler til dette. Vi har hørt kunder som trenger hjelp med å feilsøke hybrid registrerings prosessen for Azure AD JOIN under eksterne arbeids omstendigheter. Her er en analyse av hva som skjer under Vis avanserte innstillinger i løpet av registrerings prosessen.

**Sky godkjennings miljø (ved hjelp av hash-synkronisering eller direkte godkjenning av Azure AD Password)**

Denne registrerings flyten er også kjent som "Synkroniser join".

1. Windows 10 oppdager en SCP-post når brukeren logger seg på enheten.
    1. Enheten prøver først å hente leier informasjon fra klient-IDen i registeret [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Hvis den mislykkes, kommuniserer enheten med lokal Active Directory (AD) for å få leier informasjon fra tjeneste tilkoblings punkt (SCP). Hvis du vil kontrollere SCP, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Vi anbefaler å aktivere SCP i AD og bare bruke SCP for første Valide ring av klient-IDen.

2. Windows 10 prøver å kommunisere med Azure AD under system konteksten for å godkjenne seg selv mot Azure AD. Du kan kontrollere om enheten har tilgang til Microsoft-ressurser under system kontoen ved å bruke tilkoblings skriptet test enhets registrering.

3. Windows 10 genererer et selv signert sertifikat og lagrer det under data maskin objektet i lokal AD. Dette krever linje med syns vidden til domene kontrolleren.

4. Et enhets objekt som har et sertifikat, blir synkronisert til Azure AD via Azure AD Connect. Synkroniserings syklusen er hvert 30 minutt som standard, men den avhenger av konfigurasjon av Azure AD Connect. Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. På dette trinnet skal du kunne se emne enheten i tilstanden venter under enhets blad for Azure-portalen.

6. Registreringen blir fullført på den neste bruker påloggingen til Windows 10. 

> [!NOTE]
> Hvis du er på VPN og en avloggings prosess avslutter domene tilkoblingen, kan du utløse registreringen manuelt:
 1. Utsted en dsregcmd/JOIN lokalt på administrator lede tekst eller eksternt via PSExec til PC-en. For eksempel PsExec-s \\ win10client01 cmd, dsregcmd/JOIN

 2. Hvis du vil ha mer informasjon om hybrid Sammenføynings problemer, kan du se [Feilsøke enheter-problem](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
