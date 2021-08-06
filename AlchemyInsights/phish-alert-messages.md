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
ms.openlocfilehash: ac4c157d6e202488659c56605768bbfd2b3af8e658d0a2f82e529fdac6763fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999681"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Varsle e-postmeldinger fra policyen «Phish Delivered på grunn av tenant eller brukeroverstyring»

En standard varslingspolicy kalt «Phish Delivered på grunn av leier eller brukeroverstyring» er rullet ut til leiere med Microsoft Defender for Office 365 P1- og P2-lisenser. Hvis du har mottatt dette varselet, følger du fremgangsmåten nedenfor for å undersøke:

1. Klikk Vis varsel i **varselmeldingen**  for å gå til Varsler-siden i sikkerhetssenteret & samsvarssenteret.

2. Velg varselet for å se alternativet For **å vise meldingslisten** **eller Vise meldinger i Explorer**. Begge disse alternativene tar deg til detaljene i meldingen, som inkluderer meldings-ID-en. Vær oppmerksom på at Trusselutforsker-koblingen automatisk filtrerer meldingene som samsvarer med varselkriteriene. Du må kanskje justere datofilteret i Trusselutforsker.

Phishing-meldingen ble levert på grunn av en manuelt konfigurert overstyring:

- En tillatt avsender eller et domene angitt av brukeren.

- En tillatt avsender eller et domene angitt av administratoren i en policy for søppelpost.

- En tillatt IP-adresse i en policy for tilkoblingsfilter.

- En regel for e-postflyt (også kalt en transportregel) som er konfigurert til å tillate meldinger i.

Hvis du mener at meldingen ble feil merket som phish, bruker du Outlook [Rapportmelding-tillegget](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) til å sende meldingseksempler til Microsoft.
