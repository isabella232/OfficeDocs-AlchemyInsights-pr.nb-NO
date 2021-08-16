---
title: Yammer lisensieringsproblemer
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
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989742"
---
# <a name="yammer-licensing-issues"></a>Yammer lisensieringsproblemer

Alle brukere må ha en lisens for å bruke Yammer Enterprise-tjenesten, men som Yammer krever ikke at brukerne har en lisens for å få tilgang til tjenesten. Når en administrator endrer innstillingen for å blokkere Microsoft 365 brukere uten Yammer lisenser, får ikke brukere som ikke har tilordnet en Yammer Enterprise-lisens, tilgang til Yammer-tjenesten. Hvis du vil ha mer informasjon, [kan du se Administrere Yammer brukerlisenser i Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Når lisenser fjernes fra brukere, vises ikke Yammer lenger, og andre tjenester kan bruke fjerning av lisens til å skjule funksjoner. I andre tilfeller kan funksjoner fortsatt vises, men kreve lisenstilordning for å fungere.  

**Lisensen blir ikke oppdatert for brukeren**  

Noen ganger blir en bruker tilordnet en lisens, men får fremdeles ikke tilgang til Yammer. Det er mer sannsynlig at forsinkelser oppstår når en masselisenstilordning pågår. Yammer brukere kan ikke oppdateres i samme rekkefølge som lisenser endres i Azure AD fordi systemet kjører asynkront. Vent opptil 24 timer før du åpner en støttesak for å rapportere synkroniseringsproblemer med lisenser.  

**Masselisenstilordning**  

Lisenser kan tilordnes via administrasjonssenteret eller PowerShell-skripting. Hvis du vil ha mer informasjon, kan du se Tilordne [lisenser til brukere](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) og Tilordne lisenser [til brukerkontoer med Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoft Kundestøtte gir ikke hjelp med å opprette skript, men dokumentasjon Yammer lisenstilordning er tilgjengelig. Hvis du vil ha mer informasjon, [kan du se Administrere Yammer lisenser ved hjelp av Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).