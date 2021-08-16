---
title: Jeg blir blokkert av betinget tilgang med kompatibel enhet
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019157"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Jeg blir blokkert av betinget tilgang med kompatibel enhet

**Anbefalte verktøy**

- [Feilsøkingsverktøy for enhetsregistrering](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – et omfattende verktøy som hjelper deg med å feilsøke de vanligste enhetsregistreringsproblemene.
- [Test skript for tilkobling til enhetsregistrering](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – Et verktøy som brukes til å sikre at en enhet har tilgang til endepunktene for enhetsregistrering under systemkontoen.
- [Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) – Et verktøy som brukes til å søke etter og administrere foreldede enheter i miljøet.

Her er noen vanlige årsaker til at betinget tilgang mislykkes for  en kompatibel enhet, eller hvorfor brukerne kanskje mottar Du kan ikke komme dit herfra under en påloggingsforespørsel til en organisasjonsressurs.

1. **Enheten er ikke i en nødvendig enhetstilstand med en MDM:**

Bekreft at enheten er registrert hos en godkjent MDM-leverandør som Intune og *merket som kompatibel.* Hvis du vil ha mer informasjon om Intune, kan du se dette [dokumentet](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Hvis du vil ha bedre forståelse av enhetssamsvar og Intune, kan du se Bruke samsvarspolicy til å angi regler for enheter du administrerer [med Intune.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Hvis du har problemer med å registrere en enhet med Intune, kan du finne feilsøkingsdetaljer under Feilsøke enhetsregistrering [i Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Hvis du vil ha mer støtte for Intune, kan du opprette en støtteforespørsel. Dette gjør du ved å gå til [Siden Hjelp og støtte for Intune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Enheten er ikke sammenføyd med organisasjonsnettverket:**

Hvis du vil ha tilgang til organisasjonsressurser, må enheten være koblet til organisasjonens nettverk, enten via direkte tilkobling eller et virtuelt privat nettverk (VPN), og også koblet til lokale eller Azure Active Directory. Hvis du vil bli med i en arbeidsenhet i organisasjonsnettverket, kan du se Bli med i arbeidsenheten [til organisasjonens nettverk](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Hvis du vil registrere en personlig/BYOD-enhet, kan du se Registrere den [personlige enheten på organisasjonens nettverk.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Hvis du vil validere om enheten har blitt med i nettverket, kan du følge fremgangsmåten for registrerte enheter [her](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) eller arbeidsenheter [her](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Hvis du vil begrense problemet til nettverkstilkobling for organisasjonen, følger du retningslinjene nedenfor:

    1. Logg på Windows med jobb- eller skolekontoen, for eksempel alain@contoso.com.
    2. Koble til til organisasjonens nettverk via et VPN eller DirectAccess.
    3. Når du er koblet til, trykker **du Windows+L** for å låse enheten.
    4. Lås opp enheten ved hjelp av jobb- eller skolekontoen, og prøv deretter å få tilgang til den problematiske appen eller tjenesten på nytt.

Hvis du ser **feilmeldingen Du kan ikke komme** dit herfra igjen, er problemet sannsynligvis et annet sted.

3. **Operativsystemet støttes ikke:**

Kontroller at du kjører en støttet versjon av operativsystemet, inkludert:

- **Windows klient:** Windows 7 eller nyere

- **Windows Server:** Windows Server 2008 R2 eller nyere

- **macOS:** macOS X eller nyere

- **Android og iOS:** Nyeste versjon av Android- og iOS-mobiloperativsystemet

4. **Nettleser støttes ikke:**

Finn støttede nettlesere nedenfor. For Chrome-støtte med Windows 1703 eller nyere versjoner kreves en Windows 10 kontoutvidelse. For Edge 85+må brukeren være logget på for å kunne sende informasjon om enhetssamsvar på riktig måte. Hvis du vil ha mer informasjon, kan du [se her](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10:** Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1**: Internet Explorer, Chrome
- **Windows 7:** Internet Explorer, Chrome
- **iOS:** Microsoft Edge, Intune Managed Browser, Safari
- **Android:** **Microsoft Edge:** Intune Managed Browser, Chrome
- **Windows Phone:** Microsoft Edge, Internet Explorer
- **Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016:** Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2:** Internet Explorer
- **macOS:** Chrome, Safari

Finn mer informasjon om **du ikke kommer** dit-meldingen og feilsøkingstrinnene [her](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).
