---
title: 2491 varsel e-postmeldinger fra Phish leveres på grunn av leier eller bruker overstyre policyen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391420"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Varsle e-postmeldinger fra Phish leveres på grunn av leier eller bruker overstyre policyen

Et varsel som policy kalt "Phish levert på grunn av leier eller bruker overstyring" har blitt rullet til leiere med Office 365 ATP P1 og P2 lisenser. Hvis du mottok varslet, er her fremgangsmåten for å undersøke:

1. Fra varselmeldingen, klikker du **Vis varsel** for å gå til siden **varsler** i Security-& overholdelsessenteret.

2. Velg varselet for å se alternativet for å **vise meldingslisten** eller **vise meldinger i Explorer**. Begge disse alternativene tar deg til detaljer om meldingen, som inkluderer melding-ID. Vær oppmerksom på at koblingen trusselen Explorer automatisk filtrere meldinger som samsvarer med varslingskriteriene. Du må kanskje justere datofilteret i trusselen Explorer.

Phishing-melding ble levert på grunn av en overstyring av manuelt konfigurerte:

- Tillatte avsenderen eller domenet som er angitt av brukeren.

- Tillatte avsenderen eller domenet som er angitt av administrator i en policy for beskyttelse mot søppelpost.

- En tillatte IP-adresse i en tilkobling filter-policy.

- En flyt-post (også kjent som regel transport) som er konfigurert for å tillate meldinger i.

Hvis du mener at meldingen var feilaktig merket som phish bruke Outlook [rapportmelding-tillegg](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) til å sende meldingen-eksempler til Microsoft.
