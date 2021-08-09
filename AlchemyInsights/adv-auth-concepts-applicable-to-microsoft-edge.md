---
title: Avanserte godkjenningskonsepter som gjelder for Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934374"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Avanserte godkjenningskonsepter som gjelder for Microsoft Edge

Nedenfor finner du de avanserte godkjenningskonseptene som gjelder for Microsoft Edge:

**Proaktiv godkjenning**

Når du aktiverer [ProactiveAuthEnabled-policyen,](https://go.microsoft.com/fwlink/?linkid=2134621) prøver Microsoft Edge å proaktivt godkjenne påloggede brukere via Microsoft-tjenester. Med jevne mellomrom bruker den en nettbasert tjeneste til å se etter et oppdatert manifest som inneholder konfigurasjonen som styrer Proaktiv godkjenning.

Fordeler: Proaktiv godkjenning aktiverer godkjenning til viktige tjenester, for eksempel Office Ny faneside. Hvis Bing brukes som søkemotor, forbedrer proaktiv godkjenning også ytelsen til adresselinjen og bidrar til å generere søkeresultater tilpasset behovene til bedriften.

**Windows Hello CredUI for NTLM-godkjenning**

Hvis enkel pålogging (SSO) ikke er tilgjengelig når et nettsted prøver å logge på brukeren via NTLM- eller Negotiate-mekanismen, lar denne funksjonen brukeren dele OS-legitimasjonen med nettstedet og oppfylle godkjenningsutfordringen ved hjelp av Windows Hello Cred UI. Denne påloggingsflyten vises bare i Windows 10 og bare for brukere som ikke får SSO under en NTLM- eller Forhandlingsutfordring.

**Bruke lagrede passord til å logge på automatisk**

Brukere som lagrer passord i Microsoft Edge kan aktivere automatisk pålogging på nettsteder der de har lagret legitimasjon. Brukere kan aktivere eller deaktivere denne funksjonen i edge://settings/passwords, og du kan konfigurere den i [policyene for passordbehandling.](https://go.microsoft.com/fwlink/?linkid=2134622)
