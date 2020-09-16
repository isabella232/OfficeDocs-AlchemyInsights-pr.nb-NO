---
title: Løse Microsoft 365-apper finner ikke tilknyttet Office-lisenser for meldinger
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747704"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Løse Microsoft 365-appene finner ikke melding om at Office-lisenser er tilknyttet

Hvis du får denne meldingen, kan du prøve følgende:

1. Kontroller brann muren, antivirus program varen og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Microsoft 365-apper. Se [URL-adresser og IP-adresseområder for Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Fjern og [Tilordne Office-lisensen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for den aktuelle brukeren på nytt. 
3. Åpne en Office-app og [Logg](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) av eksisterende bruker kontoer.
4. Gå til Windows-innstillinger > **kontoer**  >  **e-& kontoer**, og Fjern alle arbeids kontoer unntatt den berørte kontoen.
5. Gå til Windows-innstillinger > **kontoer**  >  **få tilgang til jobb eller skole**, og koble fra alle arbeids kontoer unntatt den berørte kontoen.
6. Tilbakestill aktiveringsstatusen for Office. [Finn ut hvordan](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Logg på](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) med den berørte bruker kontoen.

Hvis du vil ha flere feil søkings løsninger, kan du se [ulisensiert produkt-og aktiverings feil i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).