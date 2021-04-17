---
title: Reparere Microsoft 365-apper Finner ikke tilknyttede office-lisenser
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
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816497"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Melding om at Microsoft 365-appene «Finner ikke tilknyttede office-lisenser»

Hvis du mottar denne meldingen, kan du prøve følgende:

1. Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Microsoft 365-apper. Se [Nettadresser og IP-adresseområder for Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Fjern og [tilordne Office-lisensen på nytt](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for den berørte brukeren. 
3. Åpne en Office-app, [og logg av](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) eventuelle eksisterende brukerkontoer.
4. Gå til Windows-innstillinger > **kontoer**& kontoer , og fjern  >  alle jobbkontoer unntatt den berørte kontoen.
5. Gå til Windows-innstillinger > **Kontoer** Tilgang til jobb eller skole , og koble fra  >  alle jobbkontoer unntatt den berørte kontoen.
6. Tilbakestill aktiveringsstatusen for Office. [Finn ut hvordan](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Logg på](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den berørte brukerkontoen.

Hvis du vil ha flere feilsøkingsløsninger, kan du [se Ulisensiert produkt og aktiveringsfeil i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).