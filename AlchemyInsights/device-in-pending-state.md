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
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914012"
---
# <a name="device-in-pending-state"></a>Enhet i ventende tilstand

**Forutsetninger:**

1. Hvis du konfigurerer enhetsregistreringer for første gang, må du kontrollere at du har gjennomgått Innføring i enhetsbehandling i [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) som veileder deg om hvordan du får enheter under kontroll av Azure AD.
2. Hvis du registrerer enheter i Azure AD direkte og registrerer dem i Intune, må du kontrollere at [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) du har konfigurert [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) og ha lisensiering på plass først.
3. Kontroller at du er autorisert til å utføre operasjoner i Azure AD og lokal AD. Bare en global administrator i Azure Active Directory kan behandle innstillinger for enhetsregistreringer. I tillegg, dersom du konfigurerer automatiske registreringer in det lokale Active Directory, må du være administrator for Active Directory og AD FS (hvis gjeldende).

Registreringsprosessen for hybrid Azure AD-sammenføyning krever at enhetene er på bedriftsnettverket. Det fungerer også over VPN, men det finnes noen begrensninger for dette. Vi har hørt at kunder trenger hjelp med feilsøking av registreringsprosessen for hybrid Azure AD-bli med under eksterne arbeidsforhold.

**Skygodkjenningsmiljø (ved hjelp av Hash-synkronisering av passord for Azure AD eller gjennomgangsgodkjenning)**

Denne registreringsflyten kalles også «Synkroniser sammenføyning».

Her er en oversikt over hva som skjer under registreringsprosessen:

1. Windows 10 oppdager SCP-posten (Service Connection Point) når brukeren logger seg på enheten.

    1. Enheten prøver først å hente leierinformasjon fra klientsidens SCP i registeret [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Hvis du vil ha mer informasjon, kan du se [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Hvis den mislykkes, kommuniserer enheten med lokal Active Directory for å få leierinformasjon fra SCP. Hvis du vil bekrefte SCP, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Vi anbefaler at du aktiverer SCP i Active Directory og bare bruker SCP på klientsiden for første validering.

2. Windows 10 prøver å kommunisere med Azure AD under systemkonteksten for å godkjenne seg selv mot Azure AD.

    Du kan kontrollere om enheten har tilgang til Microsoft-ressurser under systemkontoen ved hjelp av skriptet [Test tilkobling til enhetsregistrering](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 genererer selvsignert sertifikat og lagrer det under datamaskinobjektet i lokal Active Directory. Dette krever domenekontrollerens linje for synslinje.

4. Enhetsobjekt som har sertifikat, synkroniseres til Azure AD via Azure AD Koble til. Synkroniseringssyklusen er som standard hvert 30. minutt, men det avhenger av konfigurasjonen av Azure AD Koble til. Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. På dette stadiet skal du kunne se emneenheten i **«Ventende»** tilstand under Enhetsblad i Azure Portal.

6. Ved neste brukerpålogging Windows 10, fullføres registreringen.

    > [!NOTE]
    > Hvis du bruker VPN og avlogging/pålogging avslutter domenetilkoblingen, kan du utløse registrering manuelt. Slik gjør du det:
    >
    > Utstede en `dsregcmd /join` lokal melding på administrator eller eksternt via PSExec til PC-en.
    >
    > Eksempel: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Hvis du vil ha vanlige problemer Azure Active Directory registrering av enheter, kan du se [Vanlige spørsmål om enheter](https://docs.microsoft.com/azure/active-directory/devices/faq).
