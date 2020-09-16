---
title: Løse ulisensiert produkt-feil
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
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737962"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Forslag til å løse feil i «ulisensiert produkt»

Hvis du vil løse feil om et "ulisensiert produkt", kan du prøve følgende:

- Kontroller om abonnements statusen er utløpt.
- Kontroller at du har et abonnement som tillater klient lisenser, for eksempel Microsoft 365-apper for Business eller Business Premium, og [at brukeren har en lisens som er tilordnet](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Kontroller at brukeren logger på Office med den samme kontoen som er tilordnet lisensen.
- Kontroller [tjeneste tilstands IDen](https://docs.microsoft.com/office365/enterprise/view-service-health) for å se om det er noen kjente problemer med tjenesten.
- Kontroller brann muren, antivirus program varen og proxy-innstillingene for å bekrefte at de ikke blokkerer Microsoft 365-apper tilgang til Internet t. Se [URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Du kan også prøve følgende feil søkings handlinger: 

- Åpne en Office-app og [Logg](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) av eksisterende bruker kontoer. [Fjern](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) og [Tilordne Office-](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) lisensen på nytt, og [Logg deg](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) deretter på Office ved hjelp av den berørte bruker kontoen.
- Kjør [feil søkings verktøyet for aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Tilbakestill aktiveringsstatusen for Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Utføre en tilkoblet reparasjon av Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Hvis du trenger ytterligere feilsøkingsløsninger, kan du se: 

- [Feil ved ulisensiert produkt og aktivering i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [«Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere»-feil når du aktiverer Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)