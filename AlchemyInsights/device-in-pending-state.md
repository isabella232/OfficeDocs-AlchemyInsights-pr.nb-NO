---
title: Enhet i ventende tilstand
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679998"
---
# <a name="device-in-pending-state"></a>Enhet i ventende tilstand

**Forhånds kravene forbindelse**

1. Hvis du setter opp enhets registreringer for første gang, må du sørge for at du har gjennomgått [innføring i enhets behandling i Azure Active Directory (Azure ad)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) som hjelper deg med å få tak i enheter under kontrollen av Azure ad.
2. Hvis du registrerer enheter i Azure AD direkte og registrerer dem i Intune, må du forsikre deg om at du har [konfigurert Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) og at [lisensen](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) er på plass først.
3. Sørg for at du er autorisert til å utføre operasjoner i Azure AD og lokalt AD. Bare en global administrator i Azure AD kan administrere innstillinger for enhets registrering. Hvis du i tillegg konfigurerer automatiske registreringer i den lokale Active Directory-katalogen, må du være administrator for Active Directory og AD FS (hvis aktuelt).

Hybrid registrerings prosessen for Azure AD JOIN krever at enheter er på bedrifts nettverk. Det fungerer også over VPN, men det er noen advarsler til dette. Vi har hørt kunder som trenger hjelp med å feilsøke hybrid registrerings prosessen for Azure AD JOIN under eksterne arbeids omstendigheter.

**Sky godkjennings miljø (ved hjelp av hash-synkronisering eller direkte godkjenning av Azure AD Password)**

Denne registrerings flyten er også kjent som "Synkroniser join".

Her er en analyse av hva som skjer under registrerings prosessen:

1. Windows 10 oppdager en post for tjeneste tilkoblings punkt (SCP) når brukeren logger seg på enheten.

    1. Enheten prøver først å hente leier informasjon fra klient-IDen i registeret [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Hvis du vil ha mer informasjon, kan du se [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Hvis den mislykkes, kommuniserer enheten med lokal Active Directory for å få leier informasjon fra SCP. Hvis du vil kontrollere SCP, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Vi anbefaler å aktivere SCP i Active Directory og bare bruke SCP-IDen for den første Valide ringen.

2. Windows 10 prøver å kommunisere med Azure AD under system konteksten for å godkjenne seg selv mot Azure AD.

    Du kan kontrollere om enheten har tilgang til Microsoft-ressurser under system kontoen ved å bruke [tilkoblings skriptet test enhets registrering](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 genererer selv signert sertifikat og lagrer det under data maskin objektet i lokal Active Directory. Dette krever linje med syns vidden til domene kontrolleren.

4. Enhets objekt som har sertifikat, synkroniseres til Azure AD via Azure AD Connect. Synkroniserings syklusen er hvert 30 minutt som standard, men den avhenger av konfigurasjonen av Azure AD Connect. Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. På dette trinnet skal du kunne se emne enheten i tilstanden **venter** under enhets blad for Azure-portalen.

6. Registreringen blir fullført på den neste bruker påloggingen til Windows 10.

    > [!NOTE]
    > Hvis du er på VPN og avlogging/pålogging avslutter domene tilkoblingen, kan du utløse registreringen manuelt. Slik gjør du det:
    >
    > Utsted et `dsregcmd /join` lokalt på administrator lede tekst eller eksternt via PSExec til PC-en.
    >
    > For eksempel: `PsExec -s \\win10client01 cmd, dsregcmd /join`

For vanlige problemer med registrering av Azure Active Directory-enhet, kan du se [vanlige spørsmål om enheter](https://docs.microsoft.com/azure/active-directory/devices/faq).
