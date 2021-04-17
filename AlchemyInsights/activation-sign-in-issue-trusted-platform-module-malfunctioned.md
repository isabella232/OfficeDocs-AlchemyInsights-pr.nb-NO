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
ms.openlocfilehash: 468d197ae1ad6a3ee13cbcc683a59f0d9f193af7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822896"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Retting av Microsoft 365-appene Meldingen «Datamaskinens klarerte plattformmodul fungerer ikke som den skal»

For å løse denne filen kan du prøve følgende:

1. Åpne et Office-program og [logg av](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) eksisterende brukerkontoer.   
2. Fjern eksisterende  >  **jobbkontoer**&  >  **e-postkontoer** i Windows-innstillinger. 
3. Bruke Windows  >  **Innstillinger-kontoer**  >  **Tilgang til jobb eller skole**, koble fra eksisterende kontoer. 
4. Tilbakestill aktiveringsstatusen for Office. [Finn ut hvordan](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state
).
5. Prøv [gjenopprettingsprosessen for brukere for](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) å løse TPM-feil (Trusted Platform Module).