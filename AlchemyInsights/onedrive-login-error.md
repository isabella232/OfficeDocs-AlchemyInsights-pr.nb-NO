---
title: OneDrive påloggingsfeil AADSTS50011
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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112921"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive påloggingsfeil AADSTS50011

Hvis du får feilmeldingen «AADSTS50011: Url-adressen for svar som er angitt i forespørselen, samsvarer ikke med svaret» når du logger på OneDrive-appen, kan du se etter følgende:

Din OneDrive må være lik eller større enn versjon 20.052.XXXX.XXXX. Hvis du vil kontrollere versjonen din, klikker du det blå OneDrive-ikonet i systemstatusfeltet og **velger Hjelp & Innstillinger > Innstillinger > Om**.

Nettverket kan blokkere trafikk til **g.live.com** og **oneclient.sfx.ms**. Hvis denne trafikken er blokkert, kan OneDrive ikke oppdatere seg selv. Samarbeid med systemansvarlig for å sikre at du har tilgang til disse nettadressene. [Disse endepunktene](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) skal kunne nås for kunder som bruker Microsoft 365 abonnementer.

Hvis du trenger å få en oppdatert versjon av OneDrive manuelt, kan du gå [https://aka.ms/getonedrive](https://aka.ms/getonedrive) til .
