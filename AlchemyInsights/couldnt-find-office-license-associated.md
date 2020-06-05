---
title: Fikse Microsoft 365-apper Finner ikke tilknyttet melding om Office-lisenser
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580450"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Fikse Microsoft 365-appene "Finner ikke tilknyttede office-lisenser"

Hvis du får denne meldingen, kan du prøve følgende:

1. Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Microsoft 365-apper. Se [Url-adresser for Microsoft 365 og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Fjern og [tilordne Office-lisensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) på nytt for den berørte brukeren. 
3. Åpne en Office-app, og [logg](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) av eventuelle eksisterende brukerkontoer.
4. Gå til Windows-innstillinger > **kontoer**  >  **e-& kontoer**, og fjern alle arbeidskontoer unntatt den berørte kontoen.
5. Gå til Windows-innstillinger > **Kontoer**  >  **Få tilgang til arbeid eller skole**, og koble fra alle arbeidskontoer unntatt den berørte kontoen.
6. Tilbakestill aktiveringsstatusen for Office. [Finn ut hvordan](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Logg på](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den berørte brukerkontoen.

Hvis du vil ha flere feilsøkingsløsninger, kan du se [Ulisensiert produkt- og aktiveringsfeil i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).