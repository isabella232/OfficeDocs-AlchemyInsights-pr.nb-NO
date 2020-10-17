---
title: 726 blokkere e-postvideresending
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
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473110"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokkere eller fjerne blokkeringen av e-postvideresending

Hvis du vil aktivere eller deaktivere videre sending av e-post for en bestemt post boks, kan du se [konfigurere videre kobling](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Kontroll over ekstern videre sending utføres på leier nivå ved hjelp av den utgående søppel post policyen. Du kan kontrollere den utgående filter policyen for søppel post fra sikkerhets-og Samsvars senteret [her] ( https://protection.office.com/antispam) eller ved å bruke [Get-HostedOutboundSpamFilterPolicy-kommandoen](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).

Hvis du får følgende feil melding: **«550 5.7.520 tilgang nektet, organisasjonen tillater ikke ekstern videre sending»**, må du sørge for at policyen er konfigurert til å aktivere ekstern automatisk videre sending.

**Obs!** Det anbefales at du holder det eksterne alternativet videresendt automatisk i den standard utgående filter policyen for søppel post og aktiverer den bare for brukere som trenger ekstern videre kobling ved å opprette en egen definert policy for disse brukerne. Du kan lese mer i [konfigurere ekstern videre sending av e-post i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).