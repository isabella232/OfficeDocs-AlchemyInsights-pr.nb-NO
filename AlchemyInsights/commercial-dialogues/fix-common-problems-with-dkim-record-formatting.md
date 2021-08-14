---
title: Løse vanlige problemer med DKIM-postformatering
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 5b3dc2338843906fbc7151322b82f304b4ed04b28d8ceb349f2705c309cdeae8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930070"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Løse vanlige problemer med DKIM-postformatering

De fleste DKIM-oppsettproblemer er relatert til feil DNS-poster.

Kontroller at DKIM CNAME-posten **(ikke** en TXT-post) er riktig formatert for å løse DKIM-oppsettsproblemene. Hvis du vil ha mer informasjon, kan du se Hva du må gjøre for å konfigurere [DKIM manuelt i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Hvis du trenger hjelp med DNS-poster generelt, kan du se [Opprette DNS-poster hos en DNS-vertsleverandør for Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> Når du har opprettet eller oppdatert DKIM DNS-postene hos DNS-vertstjenesten for domenet, må du vente på at DNS-postene skal overføres.
