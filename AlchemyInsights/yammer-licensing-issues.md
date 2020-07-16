---
title: Problemer med Yammer-lisensiering
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148315"
---
# <a name="yammer-licensing-issues"></a>Problemer med Yammer-lisensiering

Alle brukere må ha en lisens til å bruke Yammer Enterprise-tjenesten, men som standard krever ikke Yammer at brukere har en lisens for å få tilgang til tjenesten. Når en administrator endrer innstillingen for å blokkere Microsoft 365-brukere uten Yammer-lisenser, får ikke brukere tilordnet en Yammer Enterprise-lisens tilgang til Yammer-tjenesten. Hvis du vil ha mer informasjon, kan du se [Administrere Yammer-brukerlisenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Når lisenser fjernes fra brukere, Yammer-flisen vises ikke lenger, og andre tjenester kan bruke lisensfjerning til å skjule funksjoner. I andre tilfeller kan funksjoner fortsatt vises, men krever lisenstilordning for å fungere.  

**Lisensen blir ikke oppdatert for brukeren**  

Noen ganger tilordnes en bruker en lisens, men får fortsatt ikke tilgang til Yammer. Forsinkelser er mer sannsynlig å oppstå når en masselisenstilordning pågår. Yammer-brukere kan ikke oppdateres i samme rekkefølge som lisenser endres i Azure AD fordi systemet kjører asynkront. Vent opptil 24 timer før du åpner en støttesak for å rapportere problemer med lisenssynkronisering.  

**Tildeling av masselisens**  

Lisenser kan tilordnes via administrasjonssenteret eller PowerShell-skripting. Hvis du vil ha mer informasjon, kan du se [Tilordne lisenser til brukere](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) og tilordne [lisenser til brukerkontoer med Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoft Support gir ikke hjelp til å opprette skript, men dokumentasjon på Yammer-lisenstilordning er tilgjengelig. Hvis du vil ha mer informasjon, kan du se [Administrere Yammer-lisenser ved hjelp av Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).