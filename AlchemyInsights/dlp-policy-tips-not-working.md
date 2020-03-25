---
title: DLP Policy Tips fungerer ikke
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932595"
---
# <a name="dlp-policy-tip-issues"></a>Problemer med dlp policy tips

**Viktig:** Mange SharePoint Online- og OneDrive-kunder kjører forretningskritiske programmer mot tjenesten som kjører i bakgrunnen. Disse inkluderer innholdsoverføring, Hindring av tap av data (DLP) og sikkerhetskopieringsløsninger. I løpet av disse enestående tider tar vi skritt for å sikre at SharePoint Online- og OneDrive-tjenester forblir svært tilgjengelige og pålitelige for brukerne som er avhengige av tjenesten mer enn noensinne i scenarier for eksternt arbeid.

Til støtte for dette målet har vi implementert strammere reguleringsgrenser for bakgrunnsapper (overførings-, DLP- og sikkerhetskopieringsløsninger) i løpet av ukedagsdagstimene. Du bør forvente at disse appene vil oppnå svært begrenset gjennomstrømning i disse tider. I løpet av kvelds- og helgetiden for regionen vil tjenesten imidlertid være klar til å behandle et betydelig høyere antall forespørsler fra bakgrunnsapper.

**Tips om DLP-retningslinjer**

Når du bruker **DLP-policyer,** kan brukere bli varslet om et brudd på retningslinjene med **policytips**. Administratorer kan konfigurere policytips som skal vises mens de tester DLP-policyen eller når policyen er i full håndhevelsesmodus.
  
Hvis du vil konfigurere policytips for DLP-policyen i sikkerhets- og samsvarssenteret i full håndhevelsesmodus, gjør du følgende:
  
- Kontroller at policytips er **aktivert** i DLP-regelen ved hjelp av trinnene [her](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

- Sørg for at **innholdet samsvarer med** det som **kreves** for å utløse regelen som er beskrevet i denne artikkelen [her](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- Policytips vises i både OWA og Outlook. Når du bruker **Outlook 2013 eller senere**, vises imidlertid policytips bare under visse forhold. Disse betingelsene er oppført her: [Støttede betingelser for Outlook 2013 eller nyere for visning av policytips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

Hvis du vil ha mer informasjon om tips om DLP-policy, kan du se: [Vise policytips for DLP-policyer](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  