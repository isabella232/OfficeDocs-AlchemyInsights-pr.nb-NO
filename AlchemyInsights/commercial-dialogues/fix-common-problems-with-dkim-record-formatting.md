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
ms.openlocfilehash: e55175e7613d220eaf956d3c7fd02213dcd5803d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323999"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a>Løse vanlige problemer med DKIM-postformatering

De fleste DKIM-oppsettproblemer er relatert til feil DNS-poster.

Kontroller at DKIM CNAME-posten **(ikke** en TXT-post) er riktig formatert for å løse DKIM-oppsettsproblemene. Hvis du vil ha mer informasjon, kan du se Hva du må gjøre for å konfigurere [DKIM manuelt i Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).

Hvis du trenger hjelp med DNS-poster generelt, kan du se [Opprette DNS-poster hos en DNS-vertsleverandør for Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

**Obs!** Når du har opprettet eller oppdatert DKIM DNS-postene hos DNS-vertstjenesten for domenet, må du vente på at DNS-postene skal overføres.
