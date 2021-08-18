---
title: Blokkere eller oppheve blokkeringen av ekstern automatisk videresending av e-post
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
ms.openlocfilehash: 6c4ddd53ab794ffad3179dd86a8f81785567cfe34240dff2aa0a1df11094883d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897477"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Blokkere eller oppheve blokkeringen av automatisk videresending av e-post

Hvis du vil aktivere eller deaktivere videresending av e-post for en bestemt postboks, kan du se [Konfigurere videresending av e-post.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Administratorer kan kontrollere ekstern videresending for organisasjonen ved hjelp [av utgående søppelpostpolicyer.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Du administrerer utgående søppelpostpolicyer i Microsoft 365 Defender-portalen på eller ved hjelp av <https://security.microsoft.com/antispam> cmdleten [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) Exchange Online PowerShell.

Hvis du får følgende feilmelding: **«550 5.7.520 Ingen tilgang,** organisasjonen tillater ikke ekstern videresending», kontroller at policyen er konfigurert til å aktivere eksterne automatisk videresendte meldinger.

**Obs!** Vi anbefaler standardverdien Automatisk –  **Systemkontrollert** for innstillingen Automatisk videresending av regler i standard policy for utgående søppelpostfilter (automatisk ekstern videresending blokkeres. Intern automatisk videresending fungerer fremdeles). Du bør opprette egendefinerte policyer for utgående søppelpostfilter og bruke verdien **På –** videresending er bare aktivert for brukere som trenger ekstern automatisk videresending av e-post. Hvis du vil ha mer informasjon, kan du se Konfigurere videresending av ekstern [e-post i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).
