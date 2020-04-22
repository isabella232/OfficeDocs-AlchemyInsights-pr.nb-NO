---
title: Flytte e-postmeldinger til Arkiv-postboksen
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
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713655"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytte e-post til arkivpostboksen

1. Bekreft at en **arkivpostboks** er aktivert. Hvis ikke, kan du bruke fremgangsmåten i [denne artikkelen](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) til å aktivere arkivpostboksen.

2. Hvis du vil arkivere meldinger automatisk til arkivpostboksen, må en oppbevaringskode med handlingen **Flytt til arkiv** angis til brukes automatisk på hele **postboksen (standard) koden**. Bruk fremgangsmåten her for å opprette taggen: [Arkiver standardkoden](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Deretter legger **Archive** du til Arkiv-taggen i oppbevaringspolicyen. I administrasjonssenteret for Exchange velger du **Oppbevaringspolicyer** > legge **til merket Flytt til arkiv** i policyen > **Lagre**.

4. Tilordne nå [oppbevaringspolicyen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den bestemte brukerens postboks. Den samme policyen vil bli brukt på både **primær-** og **arkivpostboksen.**

Det kan være nødvendig å tvinge Administrert mappeassistent (MFA) til å kjøre og bruke de nye innstillingene på brukerens postboks. Kjør følgende kommando mens [du er koblet til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for å starte administrert mappeassistent for en bestemt postboks:
  
Start-ManagedFolderAssistant -Identitet<name of the mailbox>

Hvis du vil ha mer informasjon om hvordan du konfigurerer en arkivpolicy, kan du se [Konfigurere en arkiv- og slettingspolicy for postbokser](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  