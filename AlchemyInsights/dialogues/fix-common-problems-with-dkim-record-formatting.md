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
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525651"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Løse vanlige problemer med DKIM-postformatering

De fleste DKIM-oppsettproblemer er relatert til feil DNS-poster.

Hvis du vil løse problemene med DKIM-oppsett, må du kontrollere at DKIM CNAME-posten **(ikke** en TXT-post) er formatert riktig. Hvis du vil ha mer informasjon, kan du se Hva du må gjøre [for å konfigurere DKIM manuelt i Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email)

Hvis du trenger hjelp med DNS-poster generelt, kan du se [Opprette DNS-poster hos en DNS-vert for Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

> [!NOTE]
> Når du har opprettet eller oppdatert DKIM DNS-postene hos DNS-vertstjenesten for domenet, må du vente til DNS-postene overføres.
