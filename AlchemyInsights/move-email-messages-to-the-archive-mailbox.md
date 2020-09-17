---
title: Flytte e-postmeldinger til arkiv post boksen
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
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799789"
---
# <a name="move-email-to-the-archive-mailbox"></a>Flytte e-post til arkiv post boksen

Hvis du vil at vi skal kjøre automatiske kontroller for innstillingene som nevnes nedenfor, velger du tilbake-knappen < øverst på siden, og deretter skriver du inn e-postadressen til brukeren som har problemer med å flytte e-post til arkiv post boksen.

1. Kontroller at en **arkiv post boks** er aktivert. Hvis ikke, bruker du Fremgangs måten i [denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) til å aktivere arkiv post boksen.

2. Hvis du vil arkivere meldinger automatisk til arkiv post boksen, må en oppbevarings kode med handlingen **Flytt til arkiv** være satt til **automatisk å brukes for hele post boks koden (standard)**. Bruk Fremgangs måten nedenfor for å opprette koden: [Arkiver standard-kode](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Deretter legger du til **arkiv** koden i oppbevarings policyen. I administrasjons senteret for Exchange velger du **oppbevarings policyer** for > legge til **Flytt til arkiv-koden** i policyen > **Lagre**.

4. Nå kan du [Tilordne oppbevarings policyen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den bestemte brukerens post boks. Den samme policyen vil bli brukt på både **Primær** -og **arkiv** post boksen.

Det kan være nødvendig å tvinge gjennom MFA (Managed folder Assistant) for å kjøre og bruke de nye innstillingene på brukerens post boks. Kjør følgende kommando mens du er [koblet til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for å starte den forvaltede mappe assistenten for en bestemt post boks:
  
Start-ManagedFolderAssistant-identitet <name of the mailbox>

Hvis du vil ha mer informasjon om hvordan du konfigurerer en arkiv policy, kan du se [konfigurere en policy for arkivering og sletting for post bokser](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  