---
title: 2491 Varsle e-postmeldinger fra policyen 'Phish Levert på grunn av leier eller brukeroverstyring'
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758937"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Varsle e-postmeldinger fra policyen 'Phish Levert på grunn av leier eller brukeroverstyring'

En standard varslingspolicy kalt "Phish Delivered due to tenant or user override" er rullet ut til leiere med Office 365 ATP P1- og P2-lisenser. Hvis du mottok dette varselet, er det følgende du må undersøke:

1. Klikk **Vis varsel** i varselmeldingen for å gå til **Varsler-siden** i sikkerhetssenteret for & samsvar.

2. Velg varselet for å se alternativet vise **meldingslisten** eller **Vis meldinger i Explorer**. Begge disse alternativene tar deg til detaljene i meldingen, som inkluderer meldings-ID. Vær oppmerksom på at Threat Explorer-koblingen automatisk filtrerer meldingene som samsvarer med varslingskriteriene. Du må kanskje justere datofilteret i Threat Explorer.

Phishing-meldingen ble levert på grunn av en manuelt konfigurert overstyring:

- En tillatt avsender eller domene angitt av brukeren.

- En tillatt avsender eller domene angitt av administratoren i en anti-spam-policy.

- En tillatt IP-adresse i en policy for tilkoblingsfilter.

- En postflytregel (også kjent som en transportregel) som er konfigurert til å tillate meldinger i.

Hvis du mener at meldingen ble feilaktig merket som phish, kan du bruke [Outlook-rapportmelding-tillegget](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) til å sende meldingseksempler til Microsoft.
