---
title: 305 øke størrelsen på arkiv post boksen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: 6bebc17eafd8615a6ffa95dbdf16f60768204aa7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778592"
---
# <a name="increase-the-archive-mailbox-size"></a>Øke størrelsen på arkiv post boksen


Hvis du vil at vi skal kjøre automatiserte kontroller for innstillingene som nevnes nedenfor, velger du tilbake-knappen < øverst på siden, og deretter skriver du inn e-postadressen til brukeren som har behov for å øke størrelsen på arkiv post boksen.

Microsoft 365 [begrenser](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) størrelsen på arkiv post bokser basert på lisensen som er tilordnet bruker kontoen. Når arkiv post boksen når 90% av den tillatte størrelsen, mottar brukeren et e-postvarsel. Når en arkiv post boks når størrelses grensen, kan ikke brukeren flytte flere elementer til arkiv post boksen. Microsoft 365 vil ikke øke størrelsen på en arkiv post boks når størrelses grensen er nådd. Brukere kan i stedet bruke følgende handlinger for å frigjøre plass i arkiv post boksen:

- Eksporter elementene til en. PST-fil ved hjelp av Outlook.

- Slett elementer fra arkiv post boksen.

Microsoft 365 gir **ubegrenset arkivering** for Office 365 Enterprise E3-og E5-lisenser. En administrator må aktivere denne funksjonen før arkiv-postboksen når den maksimale størrelsen. Når ubegrenset arkivering er aktivert, kan det bruke opptil 30 dager før ledig plass legges til arkiv post boksen. Derfor anbefaler vi at administratorer bekrefter den ledige plassen i arkiv post boksen, slik at brukeren kan fortsette å bruke arkiv post boksen mens den utvides. Hvis du vil ha mer informasjon, kan du se [Oversikt over ubegrenset arkivering i microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) og [aktivere ubegrenset arkivering i Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).

Hvis du vil ha mer informasjon om tilgang til arkiv post boksen fra Outlook, kan du se [Outlook-krav for å få tilgang til elementer i et automatisk utvidet arkiv](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Hvis du vil konfigurere en oppbevarings policy som automatisk flytter elementer til arkiv post boksen, kan du se [konfigurere en policy for arkivering og sletting for post bokser i Microsoft 365-organisasjonen](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Obs**! automatisk utvidelse av arkiver støttes ikke for primær post bokser på Exchange 2010.
