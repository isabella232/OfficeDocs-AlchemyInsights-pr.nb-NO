---
title: Løse Microsoft 365 apper Finner ikke tilknyttede office-lisenser
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
- "3421"
- "9001426"
ms.openlocfilehash: a65610dc5f88eeb4195e48131f08940758d0dfac0710502e0e15ab5f661c5719
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069613"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Løse meldingen Microsoft 365 «Finner ikke tilknyttede office-lisenser»

Hvis du mottar denne meldingen, kan du prøve følgende:

1. Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Microsoft 365 apper. Se [Microsoft 365 nettadresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Fjern og [tilordne Office lisensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for den berørte brukeren. 
3. Åpne en Office-app, [og logg av](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) eventuelle eksisterende brukerkontoer.
4. Gå til **Windows Innstillinger >-kontoer**  >  **E-& kontoer**, og fjern alle jobbkontoer unntatt den berørte kontoen.
5. Gå til Windows Innstillinger > **Kontoer** Tilgang til jobb eller skole , og koble fra  >  alle jobbkontoer unntatt den berørte kontoen.
6. Tilbakestill aktiveringsstatusen for Office. [Finn ut hvordan](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Logg på](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den berørte brukerkontoen.

Hvis du vil ha flere feilsøkingsløsninger, kan du [se Ulisensiert produkt og aktiveringsfeil i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).