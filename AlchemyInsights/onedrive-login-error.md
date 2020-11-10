---
title: Logg feil i OneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982484"
---
# <a name="onedrive-login-error-aadsts50011"></a>Logg feil i OneDrive AADSTS50011

Hvis du får feil meldingen «AADSTS50011: svar-URL-adressen som er angitt i forespørselen, Sams varer ikke med svaret når du logger deg på OneDrive-appen, kontrollerer du følgende:

OneDrive-versjonen må være lik eller større enn versjon 20.052. XXXX. XXXX. Hvis du vil kontrollere versjonen, klikker du på det blå OneDrive-ikonet i system status feltet, velger **hjelp & innstillinger > innstillinger > om**.

Nettverket kan blokkere trafikk til **g.live.com** og **oneclient.SFX.MS**. Hvis trafikken er blokkert, kan ikke OneDrive oppdatere seg selv. Samarbeid med nettverks administratoren for å sikre at du har tilgang til disse URL-adressene. [Disse ende punktene](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) bør nås for kunder som bruker Microsoft 365-abonnementer.

Hvis du må få en oppdatert versjon av OneDrive manuelt, kan du gå til [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
