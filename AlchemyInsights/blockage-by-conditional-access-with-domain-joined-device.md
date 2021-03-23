---
title: Jeg blir blokkert av betinget tilgang med domene sammenføyd enhet
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036703"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Jeg blir blokkert av betinget tilgang med domene sammenføyd enhet

**Anbefalte verktøy**

[Feilsøkingsverktøy for enhetsregistrering](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – verktøyet som hjelper deg med å feilsøke de vanligste registreringsproblemene for enheten.

[Test skript for tilkobling til enhetsregistrering](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – Skriptet som bidrar til å sikre at en enhet får tilgang til endepunktene for enhetsregistrering under systemkontoen.

[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) – Skriptet som lar deg søke etter og administrere foreldede enheter i miljøet.

Her er noen vanlige årsaker til at betinget tilgang kan mislykkes på en enhet som har blitt med i et domene (Hybrid Azure AD).

1. **Det er ingen Azure AD PRT** på enheten – Du må sikre at enheten har Azure AD Primary Refresh Token (PRT). Hvis du vil ha mer informasjon om PRT, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).

Hvis du vil bekrefte om du har Azure AD PRT, kan du kjøre kommandoen på enheten og kontrollere om `dsregcmd/status` «AzureAdPrt» er lik JA.

Hvis «AzureAdPrt» er «NEI», kontrollerer du følgende:

- Enten du har et forbundsmiljø med **AD FS,** og det ikke kan nås fra brukernes hjemmenettverk: I dette tilfellet må du sørge for at endepunktene «brukernavnmikset» er tilgjengelige fra ekstranettet. Hvis AD FS er bak et VPN, må du sørge for at brukerne kobler seg til VPN og logger på enheten på nytt. Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).

- **Om enhetens TPM** er feil og dermed ikke kan godkjenne enheten: Kontroller «tpm.msc» for å se om tilstanden til TPM er klar. Hvis ikke, kan `dsregcmd/leave` du kjøre og la enheten bli med i Azure AD på nytt. Prøv deretter på nytt. Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).

- **Du bruker en tredjeparts identitetsleverandør, som ikke støtter** WS-Trust protokoll . Som beskrevet i våre dokumenter, kan ikke hybrid Azure AD-sammenføyde enheter fungere i dette tilfellet. Samarbeid med identitetsleverandøren din for å få støtte.

2. Brukere bruker Chrome-nettleseren uten **Windows 10-kontoer** eller Office-utvidelse Chrome bruker ikke automatisk PRT på AAD-sammenføyde eller **hybrid-AAD-sammenføyde** enheter: Dette fører til feil i eventuelle enhetsbaserte policyer for betinget tilgang, med feilmeldingen «Uregistrert enhet» vises. Hvis du vil bruke Chrome-nettleseren på riktig måte, må du installere Windows 10-kontoer eller Office-utvidelsen til brukernes Chrome-nettleser via SCCM eller Intune. Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

Hvis det ikke er mulig å skyve utvidelsen eksternt, må du varsle brukerne om å installere en av utvidelsene ovenfor manuelt for å få tilgang til programmer bak enhetsbasert betinget tilgang. Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).

3. Enheten ble koblet til riktig hybrid Azure AD, men det ble utilsiktet slettet eller deaktivert, enten på grunn av synkroniseringsendringer i Azure AD Connect eller fra **Azure-portalen:** Hvis dette skjer, gjenkjennes ikke enhetsobjektet lenger som en fullstendig sammenføyd enhet, selv om statusen «AzureAdJoined» og «PRT» vises som gyldig på enheten.

Du kan løse dette problemet ved å `dsregcmd/leave` kjøre på de berørte enhetene og la dem bli med i Azure AD på nytt. Hvis du vil ha mer informasjon, kan du se dette [dokumentet](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).

> [!NOTE]
> Hvis enhetene er på Windows 10, 1809-oppdateringen, med VPN/Skyproxy og ser problemer med AzureAdPrt-tilstanden eller en app med SSO-problem (outlook kobler ikke til postboksen selv om du hadde PRT), må du kontrollere at du har denne oppdateringen [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) eller april kumulativ oppdatering [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) for å forhindre PRT-feil på disse maskinene.

















