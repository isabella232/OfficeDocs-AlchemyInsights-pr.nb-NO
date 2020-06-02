---
title: Flytte e-postmeldinger til arkivpostboksen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511049"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytte e-post til arkivpostboksen

1. Kontroller at en **arkivpostboks** er aktivert. Hvis ikke, kan du bruke fremgangsmåten i [denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) til å aktivere arkivpostboksen.

2. Hvis du vil arkivere meldinger automatisk til arkivpostboksen, må en oppbevaringskode med handlingen **Flytt til arkiv** settes til å brukes automatisk på hele **postbokskoden (standard).** Bruk fremgangsmåten her for å opprette koden: [Arkiver standardkode](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Deretter legger **Archive** du til Arkiv-taggen i oppbevaringspolicyen. I administrasjonssenteret for Exchange velger du **Oppbevaringspolicyer** > legge **til flytt til arkiv-koden** i policyen > **Lagre**.

4. Tilordne [nå oppbevaringspolicyen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den bestemte brukerens postboks. Den samme policyen brukes på både **primær-** og **arkivpostboksen.**

Det kan være nødvendig å tvinge administrertmappeassistent (MFA) til å kjøre og bruke de nye innstillingene på brukerens postboks. Kjør følgende kommando mens [du er koblet til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for å starte administrertmappeassistent for en bestemt postboks:
  
Start-ManagedFolderAssistant -Identitet<name of the mailbox>

Hvis du vil ha mer informasjon om hvordan du konfigurerer en arkivpolicy, kan du se [Definere en policy for arkivering og sletting for postbokser](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  