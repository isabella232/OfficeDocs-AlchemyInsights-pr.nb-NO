---
title: Problem med aktivering/pålogging – klarert plattformmodul fungerer ikke
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
- "3406"
- "9001429"
ms.openlocfilehash: 90fc3135dcde5073330abb7cfe0e45c799e2154d9cd27c075c2c9ac89c18a641
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937284"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Melding om Microsoft 365 «Datamaskinens klarerte plattformmodul fungerer ikke som den skal»

For å løse denne filen kan du prøve følgende:

1. Åpne et Office-program og [logg av](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) eksisterende brukerkontoer.   
2. Bruk Windows **Innstillinger**  >  **kontoer**  >  **E-& kontoer**, fjern eksisterende jobbkontoer. 
3. Bruk Windows **Innstillinger**  >  **kontoer**  >  **Tilgang til jobb eller skole**, koble fra eksisterende kontoer. 
4. Tilbakestill aktiveringsstatusen for Office. [Finn ut hvordan](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).
5. Prøv [gjenopprettingsprosessen for brukere for](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) å løse TPM-feil (Trusted Platform Module).