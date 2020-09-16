---
title: Problemer med Yammer-lisensiering
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657285"
---
# <a name="yammer-licensing-issues"></a>Problemer med Yammer-lisensiering

Alle brukere må ha en lisens for å bruke Yammer Enterprise-tjenesten, men som standard er Yammer ikke nødvendig for at brukere har en lisens for å få tilgang til tjenesten. Når en administrator endrer innstillingen for å blokkere Microsoft 365-brukere uten Yammer-lisenser, får ikke brukere tilordnet en Yammer Enterprise-lisens til å få tilgang til Yammer-tjenesten. Hvis du vil ha mer informasjon, kan du se [administrere bruker lisenser for Yammer i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Når lisenser er fjernet fra brukere, vises ikke lenger Yammer-delark, og andre tjenester kan bruke fjerning av lisenser til å skjule funksjoner. I andre tilfeller kan funksjoner fortsatt vises, men krever lisens tilordning for å fungere.  

**Lisensen blir ikke oppdatert for brukeren**  

Noen ganger er en bruker tilordnet en lisens, men har fremdeles ikke tilgang til Yammer. Det er mer sannsynlig at forsinkelser oppstår når en masse lisens tildeling pågår. Yammer-brukere blir kanskje ikke oppdatert i samme rekkefølge som lisenser endres i Azure AD fordi systemet kjører asynkront. Vent opptil 24 timer før du åpner en støtte sak for å rapportere synkroniserings problemer med lisenser.  

**Masse lisens tilordning**  

Lisenser kan tildeles gjennom administrasjons senteret eller PowerShell-skript. Hvis du vil ha mer informasjon, kan du se [Tilordne lisenser til brukere](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) og [Tilordne lisenser til bruker kontoer med Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoft kunde støtte gir ikke hjelp til å opprette skript, men dokumentasjon om Yammer-lisens tildeling er tilgjengelig. Hvis du vil ha mer informasjon, kan du se [administrere Yammer-lisenser ved hjelp av Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).