---
title: Problemer med å logge på Microsoft 365-apper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695332"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Løse Microsoft 365-appene "Beklager, en annen konto fra organisasjonen er allerede logget på" melding

For å løse denne filen kan du prøve følgende:

- Fjern alle arbeids kontoer, unntatt den berørte kontoen, ved hjelp av Windows-innstillinger > **få tilgang til jobb eller skole**.
- [Fjern Office-legitimasjon](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows-legitimasjons behandling.<br/>
    **Obs!** Register banene for Office 2016 har blitt endret til 16,0. (Eks: \Software\Microsoft\Office\16.0\Common\Identity\)
- Åpne en Office-app, **File**og velg  >  **Account**  >  **Logg på**fil konto. Logg deretter på med en bruker konto med en gyldig lisens. Hvis du vil ha mer informasjon, se [Kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Hvis du bruker Mac, kan du ta en titt på [Jeg kan ikke logge på en Office 2016 for Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Hvis du vil ha mer informasjon, kan du se ["Beklager, en annen konto fra organisasjonen er allerede logget på denne data maskinen" i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).