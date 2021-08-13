---
title: Flytte e-postmeldinger til arkivpostboksen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974966"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytte e-post til arkivpostboksen

Hvis du vil at vi skal kjøre automatiserte kontroller for innstillingene som er nevnt nedenfor, velger du Tilbake-knappen <- øverst på denne siden, og deretter skriver du inn e-postadressen til brukeren som har problemer med å flytte e-post til arkivpostboksen.

1. Bekreft at en **arkivpostboks** er aktivert. Hvis ikke, kan du bruke fremgangsmåten i [denne artikkelen til](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) å aktivere arkivpostboksen.

2. Hvis du vil arkivere meldinger automatisk i  arkivpostboksen, må en oppbevaringskode med handlingen Flytt til arkiv angis til å brukes automatisk på hele postboksen **(standard)-koden**. Bruk fremgangsmåten her for å opprette koden: [Arkivstandardkode](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Deretter legger du til **Arkiv-koden** i oppbevaringspolicyen. I administrasjonssenteret Exchange velger du Oppbevaringspolicyer **>** legg til Flytt til arkiv-koden i policyen >  **Lagre**.

4. Tilordne [oppbevaringspolicyen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den bestemte brukerens postboks. Den samme policyen brukes på både **primær-** og **arkivpostboksen.**

Det kan være nødvendig å tvinge assistenten for administrert mappe (MFA) til å kjøre og bruke de nye innstillingene på brukerens postboks. Kjør følgende kommando mens du [er koblet til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for å starte assistenten for administrert mappe for en bestemt postboks:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Hvis du vil ha mer informasjon om hvordan du konfigurerer en arkivpolicy, kan du se Konfigurere en policy for arkivering og [sletting for postbokser](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  