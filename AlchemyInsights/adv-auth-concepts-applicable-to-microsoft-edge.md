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
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398594"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Avanserte godkjenningskonsepter som gjelder for Microsoft Edge

Nedenfor finner du de avanserte godkjenningskonseptene som gjelder for Microsoft Edge:

**Proaktiv godkjenning**

Når du aktiverer [ProactiveAuthEnabled-policyen,](https://go.microsoft.com/fwlink/?linkid=2134621) prøver Microsoft Edge å proaktivt godkjenne påloggede brukere via Microsoft-tjenester. Med jevne mellomrom bruker den en nettbasert tjeneste til å se etter et oppdatert manifest som inneholder konfigurasjonen som styrer Proaktiv godkjenning.

Fordeler: Proaktiv godkjenning gjør det mulig å godkjenning til viktige tjenester, for eksempel Office Ny fane-siden. Hvis Bing brukes som søkemotor, forbedrer proaktiv godkjenning også ytelsen til adresselinjen og bidrar til å generere søkeresultater tilpasset behovene til bedriften.

**Windows Hello CredUI for NTLM-godkjenning**

Hvis enkel pålogging (SSO) ikke er tilgjengelig når et nettsted prøver å logge på brukeren via NTLM- eller Negotiate-mekanismen, lar denne funksjonen brukeren dele OS-legitimasjonen med nettstedet og oppfylle godkjenningsutfordringen ved hjelp av Windows Hello Cred-brukergrensesnittet. Denne påloggingsflyten vises bare i Windows 10 og bare for brukere som ikke får SSO under en NTLM- eller Forhandlingsutfordring.

**Bruke lagrede passord til å logge på automatisk**

Brukere som lagrer passord i Microsoft Edge, kan aktivere automatisk pålogging på nettsteder der de har lagret legitimasjon. Brukere kan aktivere eller deaktivere denne funksjonen i edge://settings/passwords, og du kan konfigurere den i [policyene for passordbehandling.](https://go.microsoft.com/fwlink/?linkid=2134622)
