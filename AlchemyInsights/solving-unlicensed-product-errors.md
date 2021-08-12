---
title: Løse ulisensiert produkt-feil
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
- "3412"
- "9001428"
ms.openlocfilehash: 7922a2c5306f9d16856502b5e57e585cb90f2f7c9abaad0366f72ed46de786d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957109"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Forslag til å løse ulisensiert produkt-feil

Hvis du vil løse feil om et ulisensiert produkt, kan du prøve følgende:

- Kontroller om abonnementsstatusen er utløpt.
- Kontroller at du har et abonnement som tillater klientlisenser, for eksempel Microsoft 365 Apps for business eller Business Premium, og kontroller at brukeren har [en tilordnet lisens](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Kontroller at brukeren logger på Office med den samme kontoen som har lisensen tilordnet.
- Se siden [tjenestetilstand for](https://docs.microsoft.com/office365/enterprise/view-service-health) å se om det er noen kjente problemer med tjenesten.
- Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Microsoft 365 apper tilgang til Internett. Se [nettadresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Du kan også prøve følgende feilsøkingshandlinger: 

- Åpne en Office-app, [og logg av](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) eventuelle eksisterende brukerkontoer. [Fjern](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) og [tilordne Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) lisensen på nytt, og logg deretter på Office [den](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) berørte brukerkontoen.
- Kjør feilsøking [for aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Tilbakestill aktiveringsstatusen for Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Utføre en tilkoblet reparasjon av Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Hvis du trenger ytterligere feilsøkingsløsninger, kan du se: 

- [Feil ved ulisensiert produkt og aktivering i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [«Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere»-feil når du aktiverer Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)