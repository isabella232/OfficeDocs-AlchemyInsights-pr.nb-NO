---
title: 305 øke størrelsen på postboksen arkiv
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: 28086145d8769bd06ef6352257a820146c5f237d
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391425"
---
# <a name="increase-the-archive-mailbox-size"></a>Øke størrelsen på postboksen arkiv

Office 365 [begrenser](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) størrelsen på arkivet postbokser basert på lisensen som er tilordnet brukerkontoen. Når postboksen arkiv når 90% av den tillatte størrelsen, mottar brukeren en e-postmelding. Når en arkiv-postboks når størrelsesgrensen, kan ikke brukeren flytte flere elementer til arkiv-postboks. Office 365 vil ikke øke størrelsen på en arkiv-postboks når størrelsesgrensen er nådd. I stedet, kan brukere ta følgende forholdsregler for å frigjøre plass i postboksen arkiv:

- Eksport av elementer til en PST-fil ved hjelp av Outlook

- Slette elementer fra postboksen arkiv.

Office 365 gir **ubegrenset arkivering** for Office 365 Enterprise E3 og E5 lisenser. En administrator må aktivere denne funksjonen før postboksen arkiv har nådd sin maksimale størrelse. Når ubegrenset arkivering er aktivert, kan det ta opptil 30 dager før ledig plass som er lagt til arkiv-postboks. Derfor anbefaler vi at administratorer kontrollerer ledig plass i postboksen arkiv, som tillater brukeren å fortsette å bruke arkiv-postboks mens den utvides. Hvis du vil ha mer informasjon, se [Oversikt over ubegrenset arkivering i Office 365](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving) og [aktivere ubegrenset arkivering i Office 365](https://docs.microsoft.com/office365/securitycompliance/enable-unlimited-archiving).

Hvis du vil ha mer informasjon om tilgang til arkivet postboksen fra Outlook, kan du se [krav til Outlook for å få tilgang til elementer i en auto-utvidet arkiv](https://docs.microsoft.com/office365/securitycompliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Hvis du vil konfigurere en oppbevaringspolicy som automatisk flytter elementer til arkiv-postboksen, kan du se [Konfigurere en policy for arkivering og sletting for postbokser i Office 365-organisasjon](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Merknad**: Autoutvidelse Arkiver støttes ikke for primære postbokser i Exchange 2010.
