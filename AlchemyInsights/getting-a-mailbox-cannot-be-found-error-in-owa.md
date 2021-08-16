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
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056499"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Finner du ikke en postboksfeil i Outlook på nettet?

Hvis du bruker Outlook på nettet, og du får en Postboks ble ikke funnet **for** feil, har ikke kontoen som du brukte til å koble til Outlook på nettet, en Exchange Online-lisens, og derfor er ingen postboks knyttet til kontoen. Administratoren kan tilordne en lisens til kontoen din ved å følge disse trinnene:

1. Åpne [Administrasjonssenter for Microsoft 365](https://portal.office.com/adminportal/home#/homepage) og gå til **Aktive brukere** under **Brukere-delen,** og velg brukeren som ser feilen.

2. Gå til Lisenser og apper-delen på brukersiden som  åpnes, velg riktig **plasseringsverdi,** og tilordne en lisens som inneholder Exchange Online (utvid lisensen for å se detaljene). Når du er ferdig, klikker du **Lagre endringer**.

I noen tilfeller, hvis lisensen allerede er tilordnet til en brukerkonto, bidrar fjerning og tilordning av lisensen til å løse problemet og få den klargjort på riktig måte i systemet: 

- Kontroller om M365-abonnementet Exchange Online (og andre, hvis du har noen) abonnementer som er oppdaterte og ikke nylig utløpt.

Når du har forsikret deg om at abonnementet ikke er utløpt og en gyldig lisens er tilordnet til brukerkontoen, kan det ta opptil 24 timer før lisensen blir klargjort, så du må kanskje vente på at problemet skal løses. Hvis du vil ha mer informasjon, [kan du se Tilordne og administrere lisenser](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).