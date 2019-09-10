---
title: Flytt e-postmeldinger til arkiv-postkassen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822171"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytt e-post til arkivpostboksen

1. Kontroller at en **arkivpostboks** er aktivert. Hvis ikke, bruker du fremgangsmåten i [denne artikkelen](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) til å aktivere arkiv-postboksen.

2. Hvis du vil arkivere meldinger automatisk til arkivpostboksen, må en oppbevaringskode med **Flytt til arkiv** -handlingen settes til å **brukes automatisk på hele postboks koden (standard)**. Bruk fremgangsmåten her for å opprette taggen: [Arkiver standardkode](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Deretter legger du til **arkiv** koden i oppbevaringspolicyen. I administrasjonssenteret for Exchange velger du **oppbevaringspolicyer** > legger til **Flytt til arkiv-koden** i policyen > **Lagre**.

4. Nå kan du [Tilordne oppbevaringspolicyen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den bestemte brukerens postboks. Den samme policyen vil bli brukt både på **Primær** -og **arkiv** postboksen.

Det kan være nødvendig å tvinge administrert Mappeassistent (MFA) til å kjøre og bruke de nye innstillingene til brukerens postboks. Kjør følgende kommando mens du er [koblet til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) til å starte assistenten for administrerte mapper for en bestemt postboks:
  
Start-ManagedFolderAssistant-identitet<name of the mailbox>

Hvis du vil ha mer informasjon om hvordan du konfigurerer en arkiveringspolicy, kan du se [konfigurere en arkiverings-og slettings policy for postbokser](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  