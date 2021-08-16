---
title: Domenestatus – Ingen tjenester er valgt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 1476a88c7b974a9e6cfe443f6842df8cdc3d7073a73c0add7e6f183dd0528de1
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57874404"
---
# <a name="domain-status---no-services-selected"></a>Domenestatus – Ingen tjenester er valgt

Ingen tjenester valgt **betyr** at du ikke har valgt noen Microsoft 365-tjenester, for eksempel Exchange Online, Skype for Business eller Intune, og Administrasjon av mobilenheter for Microsoft 365 kan brukes med det egendefinerte domenet. Hvis du bruker Exchange Hybrid (Exchange lokalt med Exchange Online) eller ekstern søppelpostfiltrering med Exchange og ingen andre Microsoft-tjenester, kan du ignorere denne meldingen. Status for domenetilstand er bare tilgjengelig for domener som er koblet direkte til tjenesten.

Slik velger du tjenester for domenet:

1. Merk **Innstillinger** av for domenet med statusmeldingen Ingen tjenester valgt fra Innstillinger  >  [](https://admin.microsoft.com/Adminportal/Home) **Domener**.
1. Velg **Administrer DNS for** å starte veiviseren for domeneoppsett.
    - Hvis du velger **Legg til dine egne DNS-poster**, må du passe på å velge en tjeneste når du blir bedt om det. Flere tjenester kan være tilgjengelige under **Avanserte alternativer**.
    - Hvis du velger La Microsoft  **legge til DNS-postene** eller Flere alternativer Konfigurer nettjenestene mine for meg, foreslås alle tilgjengelige tjenester og  >   velges automatisk.
1. Fortsett gjennom veiviseren for å fullføre DNS-konfigurasjonen og tjenestevalgene.
 
Hvis du vil ha mer hjelp med å konfigurere domenet, kan du se Legge til [DNS-poster for å koble til domenet.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

