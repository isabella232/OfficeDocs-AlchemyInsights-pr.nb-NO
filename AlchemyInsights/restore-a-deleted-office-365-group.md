---
title: Gjenopprette en slettet Microsoft 365-gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645140"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>Gjenopprette en slettet Microsoft 365-gruppe

Du kan gjenopprette en slettet Microsoft 365-gruppe eller Microsoft Teams innen 30 dager etter slettingen.

1. Gå til [administrasjonssenteret for Microsoft 365](https://aka.ms/RestoreDeletedGroup) for å logge på en liste over slettede grupper og team.

    **Obs!** Logg på med kontoen som er tilordnet til enten leieradministratoren eller administratorrollen for gruppene.

1. Velg den slettede Microsoft 365-gruppen/Teams som skal gjenopprettes, og klikk **gjenopprett gruppe.**

    Hvis gruppen ikke kan gjenopprettes på grunn av en motstridende SMTP-adresse, bruker du følgende kommando til å finne objektet som forårsaker konflikt, og fjerne SMTP-adressen:

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **Obs!** I noen tilfeller kan det ta så lang tid som 24 timer før gruppen og alle dataene gjenopprettes.

    Hvis du vil ha mer informasjon, eller hvis du vil lære hvordan du gjenoppretter grupper ved hjelp av PowerShell, kan du se Gjenopprette en [slettet Microsoft 365-gruppe.](https://go.microsoft.com/fwlink/?linkid=867802)