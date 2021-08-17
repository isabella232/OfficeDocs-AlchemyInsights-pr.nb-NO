---
title: 726 Blokkere videresending av e-post
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059641"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokkere eller oppheve blokkering av videresending av e-post

Hvis du vil aktivere eller deaktivere videresending av e-post for en bestemt postboks, kan du se [Konfigurere videresending av e-post.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

På tenantnivå utføres kontroll av ekstern videresending ved hjelp av policyen for utgående søppelpost. Du kan sjekke policyen for utgående søppelpostfilter fra Sikkerhets- og samsvarssenteret [her](https://protection.office.com/antispam) eller ved hjelp av [kommandoen Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Hvis du får følgende feilmelding: **«550 5.7.520 Ingen tilgang,** organisasjonen tillater ikke ekstern videresending». Kontroller at policyen er konfigurert til å aktivere ekstern automatisk videresending.

**Obs!** Det anbefales å la ekstern autoforward være deaktivert på standard policy for utgående søppelpostfilter og aktivere den bare for brukere som trenger ekstern videresending, ved å opprette en egendefinert policy for disse brukerne. Du kan lese mer i Konfigurere videresending av [ekstern e-post i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).