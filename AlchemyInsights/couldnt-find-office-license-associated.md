---
title: Fikse Office-apper Finner ikke tilknyttede office-lisenser
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
ms.openlocfilehash: 565df0a05baa974a6cbac58ac6be8d78470dbc5d
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715641"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a>Fikse meldingen Office-apper "Finner ikke office-lisenser knyttet"

Hvis du mottar denne meldingen, kan du prøve følgende:

1. Kontroller brannmur-, antivirusprogramvaren- og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Office-apper. Se [Url-adresser og IP-adresseområder for Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Fjern og [tilordne Office-lisensen](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) på nytt for den berørte brukeren. 
3. Åpne en Office-app, og [logg av](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) eventuelle eksisterende brukerkontoer.
4. Gå til Windows-innstillinger > **Kontoer** > **E-post & kontoer**, og fjern alle arbeidskontoer unntatt den berørte kontoen.
5. Gå til Windows-innstillinger > **Kontoer** > **Access-arbeid eller skole**, og koble fra alle arbeidskontoer unntatt den berørte kontoen.
6. Tilbakestill aktiveringstilstanden for Office. [Finn ut hvordan](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Logg på](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den berørte brukerkontoen.

Hvis du vil ha flere løsninger for feilsøking, kan du se [Ulisensiertprodukt- og aktiveringsfeil i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).