---
title: Behandle nettseminarregistrering
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793913"
---
# <a name="manage-webinar-registration"></a>Behandle nettseminarregistrering

Du administrerer hvem som kan registrere seg Teams webinarer ved å Teams Powershell-kommandoer. Hvis du vil Teams Powershell, [kan du Teams PowerShell](/microsoftteams/teams-powershell-install). 

Som standard *er WhoCanRegister* aktivert og satt til **EveryoneInCompany**. Hvis du vil tillate at alle, inkludert anonyme brukere, kan registrere seg, må du angi møtepolicyen til **Alle** ved hjelp av Powershell-kommandoen:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Obs!** Hvis anonym sammenføyning er deaktivert i møteinnstillingene, kan ikke anonyme brukere bli med i nettseminarer. Hvis du vil lære mer og aktivere denne innstillingen, kan du se [Behandle møteinnstillinger i Microsoft Teams](/microsoftteams/meeting-settings-in-teams).

Hvis du vil deaktivere møteregistrering, setter du *AllowMeetingRegistration til* **False**.

Hvis du vil lære mer om hvordan du konfigurerer hvem som kan registrere seg for nettseminarer, kan du se Konfigurere hvem som [kan registrere seg for nettseminarer](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Hvis du vil ha mer informasjon om innstillinger for Microsoft-lister, kan [du se Kontrollere innstillinger for Microsoft-lister](/sharepoint/control-lists).
