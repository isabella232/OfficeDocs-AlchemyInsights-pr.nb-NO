---
title: Avanserte godkjennings begreper som gjelder for Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573525"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Avanserte godkjennings begreper som gjelder for Microsoft Edge

Følgende er de avanserte godkjennings konseptene som gjelder for Microsoft Edge:

**Proaktiv godkjenning**

Når du aktiverer [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) -policyen, vil Microsoft Edge prøve å godkjenne påloggede brukere via Microsoft-tjenester. Med regelmessige intervaller vil det bruke en nett BAS ert tjeneste til å se etter et oppdatert manifest som inneholder konfigurasjonen som styrer proaktiv godkjenning.

Fordeler: proaktiv godkjenning muliggjør godkjenning for viktige tjenester, for eksempel siden for ny fane i Office. Hvis Bing brukes som søke motor, forbedrer proaktivt godkjenning ytelsen på adresse linjen og bidrar til å generere søke resultater tilpasset behovene til bedriften.

**Windows Hello-CredUI for NTLM-godkjenning**

Hvis Single Sign-on (SSO) ikke er tilgjengelig når et nettsted prøver å logge på brukeren gjennom NTLM-eller Negotiate-mekanismen, kan denne funksjonen dele OS-legitimasjonen med nettstedet og oppfylle godkjennings utfordringen ved hjelp av Windows Hello-legitimasjons bruker grensesnittet. Denne flyten vises bare i Windows 10, og bare for brukere som ikke får SSO under en NTLM eller en Negotiate-utfordring.

**Bruke lagrede passord til å logge på automatisk**

Brukere som lagrer passord i Microsoft Edge, kan aktivere automatisk pålogging til nett steder der de har lagret legitimasjon. Brukere kan aktivere eller deaktivere denne funksjonen i edge://settings/passwords, og du kan konfigurere den i policyer for [passord behandling](https://go.microsoft.com/fwlink/?linkid=2134622) .
