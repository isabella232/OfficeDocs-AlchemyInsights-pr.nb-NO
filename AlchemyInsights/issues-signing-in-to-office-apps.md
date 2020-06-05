---
title: Problemer med å logge på Microsoft 365-apper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579946"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Fikse Microsoft 365 apps "Beklager, en annen konto fra organisasjonen er allerede logget på" melding

For å løse denne filen kan du prøve følgende:

- Fjern alle arbeidskontoer, unntatt den berørte kontoen, ved hjelp av Windows-innstillinger > **Access-arbeid eller skole**.
- [Fjern Office-legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows Legitimasjonsbehandling.<br/>
    **Merk:** Registerbanene for Office-2016 er endret til 16.0. (Eks: \Software\Microsoft\Office\16.0\Common\Identity\)
- Åpne en Office-app, velg **Logg**av  >  **filkonto**  >  **Sign Out**. Logg deretter på med en brukerkonto med en gyldig lisens. Hvis du vil ha mer informasjon, se [Kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Hvis du bruker Mac, kan du ta en titt på [Jeg kan ikke logge på en Office 2016 for Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Hvis du vil ha mer informasjon, kan du se ["Beklager, en annen konto fra organisasjonen er allerede logget på denne datamaskinen" i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).