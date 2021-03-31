---
title: Finner du ikke feilen 126 Får du en postboks i OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426671"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Finner du ikke en postboksfeil i Outlook på nettet?

Hvis du bruker Outlook på nettet og du får en Postboks ble ikke funnet **for** feil, har ikke kontoen som du brukte til å koble til Outlook på nettet, en Exchange Online-lisens, og derfor er ingen postboks knyttet til kontoen. Administratoren kan tilordne en lisens til kontoen din ved å følge disse trinnene:

1. Åpne [administrasjonssenteret for Microsoft 365,](https://portal.office.com/adminportal/home#/homepage)  gå til **Aktive** brukere under Brukere-delen, og velg brukeren som ser feilen.

2. Gå til Lisenser og apper-delen på brukersiden som  åpnes, velg riktig **plasseringsverdi,** og tilordne en lisens som inneholder Exchange Online (utvid lisensen for å se detaljene). Når du er ferdig, klikker du **Lagre endringer**.

I noen tilfeller, hvis lisensen allerede er tilordnet til en brukerkonto, bidrar fjerning og tilordning av lisensen til å løse problemet og få den klargjort på riktig måte i systemet: 

- Kontroller om M365 Exchange Online (og andre, hvis du har noen) abonnementer er oppdaterte og ikke nylig utløpt.

Når du har forsikret deg om at abonnementet ikke er utløpt og en gyldig lisens er tilordnet til brukerkontoen, kan det ta opptil 24 timer før lisensen blir klargjort, så du må kanskje vente på at problemet skal løses. Hvis du vil ha mer informasjon, [kan du se Tilordne og administrere lisenser](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).