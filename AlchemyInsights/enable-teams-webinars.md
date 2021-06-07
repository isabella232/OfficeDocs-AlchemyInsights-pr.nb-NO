---
title: Aktivere Teams webinarer
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793784"
---
# <a name="enable-teams-webinars"></a>Aktivere Teams webinarer

Webinarer er aktivert som standard. Du kan administrere hvem som kan planlegge og registrere seg for Teams webinarer ved å Teams PowerShell-kommandoer.

- Alle brukere som kan opprette et møte, kan også opprette et nettseminarmøte. Hvis du vil administrere hvem som kan planlegge Teams webinarer, bruker du *AllowMeetingRegistration*. 
- Som standard *er WhoCanRegister* aktivert og satt til **Alle**. Hvis du vil deaktivere møteregistrering, setter du *AllowMeetingRegistration til* **False**.

Hvis du vil endre disse innstillingene, må du [installere Teams PowerShell](/microsoftteams/teams-powershell-install). Møtepolicyer håndheves også på Teams webinarer. Hvis for eksempel anonym sammenføyning er deaktivert i møteinnstillingene, kan anonyme brukere ikke bli med i nettseminarer.

Hvis du vil lære mer om hvordan du konfigurerer hvem som kan registrere seg for nettseminarer, kan du se Konfigurere hvem som [kan registrere seg for nettseminarer](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars). Hvis du vil ha mer informasjon om innstillinger for Microsoft-lister, kan [du se Kontrollere innstillinger for Microsoft-lister](/sharepoint/control-lists).