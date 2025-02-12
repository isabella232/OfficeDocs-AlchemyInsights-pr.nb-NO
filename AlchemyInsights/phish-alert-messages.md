---
title: 2491 Varsle e-postmeldinger fra policyen «Phish Delivered på grunn av tenant eller brukeroverstyring»
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316367"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Varsle e-postmeldinger fra policyen «Phish Delivered på grunn av tenant eller brukeroverstyring»

En standard varslingspolicy kalt **Phish Delivered** på grunn av leier- eller brukeroverstyring er tilgjengelig i organisasjoner med Microsoft Defender for Office 365 P1- og P2-lisenser. Hvis du har mottatt dette varselet, følger du fremgangsmåten nedenfor for å undersøke:

1. Klikk Vis varsel i **varselmeldingen** for å gå til **Varsler-siden** i Microsoft 365 Defender portalen.

2. Velg varselet for å se alternativet For **å vise meldingslisten** **eller Vise meldinger i Explorer**. Begge disse alternativene tar deg til detaljene i meldingen, som inkluderer meldings-ID-en. Vær oppmerksom på at Trusselutforsker-koblingen automatisk filtrerer meldingene som samsvarer med varselkriteriene. Du må kanskje justere datofilteret i Trusselutforsker.

Phishing-meldingen ble levert på grunn av en manuelt konfigurert overstyring:

- En tillatt avsender eller et domene angitt av brukeren.
- En tillatt avsender eller et domene som er angitt av administratoren i en policy for søppelpost.
- En tillatt IP-adresse i en policy for tilkoblingsfilter.
- En regel for e-postflyt (også kalt en transportregel) som er konfigurert til å tillate meldinger i.

Hvis du mener at meldingen ble feil merket som phishing, kan du bruke [Administratorinnsending](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) til å rapportere meldingen til Microsoft.

Brukere kan bruke [tillegget Rapportmelding](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) eller Tilleggsprogrammet Rapporter phishing til å Outlook sende meldingseksempler til Microsoft.
