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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219864"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokkere eller fjerne blokkeringen av e-postvideresending

Hvis du vil aktivere eller deaktivere videre sending av e-post for en bestemt post boks, kan du se [konfigurere videre kobling](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Kontroll over ekstern videre sending utføres på leier nivå ved hjelp av den utgående beskyttelses policyen for søppel post. Hvis den er satt til av eller automatisk, kan det blokkere e-postvideresending med tilgangs meldingen "550 5.7.520 ingen tilgang, organisasjonen tillater ikke ekstern videre sending". Hvis videre sending ble satt til blokkert, og det er feilen brukerne vil se.

Hvis videre sending blir blokkert, må du kontrollere at policyen er konfigurert til å aktivere ekstern automatisk videre sending. Du kan kontrollere den utgående filter policyen for søppel post fra sikkerhets-og Samsvars senteret eller ved å kjøre kommandoen Get-HostedOutboundSpamFilterPolicy | fl-navn, AutoForwardingMode. Hvis du vil konfigurere automatisk videre sending, vil den samme kommandoen fortelle deg tilstanden til policyen nå.

Obs! det anbefales at du holder det eksterne alternativet videresendt automatisk i den standard utgående filter policyen for søppel post og aktiverer den bare for brukere som trenger ekstern videre sending ved å opprette en egen definert policy for disse brukerne. Du kan lese mer i [konfigurere ekstern videre sending av e-post i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).