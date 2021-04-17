---
title: Problemer med å logge på Microsoft 365-apper
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833084"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Løse meldingen «Beklager, en annen konto fra organisasjonen er allerede pålogget» i Microsoft 365-appene

For å løse denne filen kan du prøve følgende:

- Fjern alle jobbkontoer, bortsett fra den berørte kontoen, ved hjelp av Windows-innstillinger > **Access jobb eller skole**.
- [Fjern Office-legitimasjon ved hjelp](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) av Windows Legitimasjonsbehandling.<br/>
    **Obs!** Registerbanene for Office 2016 er endret til 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Åpne en Office-app, og **velg Logg** av  >    >  **filkonto**. Logg deretter på med en brukerkonto med en gyldig lisens. Hvis du vil ha mer informasjon, se [Kontoer i Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Hvis du bruker Mac, kan du ta en titt på [Jeg kan ikke logge på en Office 2016 for Mac-app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Hvis du vil ha mer informasjon, kan du se «Beklager, en annen konto fra organisasjonen er allerede logget på [denne datamaskinen» i Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).