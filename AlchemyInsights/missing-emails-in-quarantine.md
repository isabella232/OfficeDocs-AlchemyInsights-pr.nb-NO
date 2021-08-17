---
title: Manglende e-postmeldinger i karantene
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: bd5a04fd5abad962b4e85e009a9232e1a93219c238c629506df5cfb034453df2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57892056"
---
# <a name="missing-emails-in-quarantine"></a>Manglende e-postmeldinger i karantene

Administratorer kan [vise, frigi eller slette disse meldingene](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Gå til Se gjennom karantene i Microsoft 365 Defender <https://security.microsoft.com>  \> **portalen** på . Du kan også gå direkte til **Karantene-siden** ved å bruke <https://security.microsoft.com/quarantine> .  

Hvis du vil ha mer informasjon om søke-/filterverdiene du kan bruke, kan du se Behandle meldinger og filer i [karantene](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)som administrator i EOP .

Cmdletene du bruker til å vise og behandle meldinger og filer i karantene, er:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Vær oppmerksom på at denne cmdleten bare er for meldinger, ikke filer fra Safe-vedlegg for SharePoint, OneDrive eller Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
