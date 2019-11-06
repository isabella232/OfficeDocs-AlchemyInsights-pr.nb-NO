---
title: 2609-oppbevaring-eller-eDiscovery-Hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994082"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a>Kan ikke slette elementer i SharePoint Online eller OneDrive for bedrifter

Du eller brukerne kan ikke slette elementer i SharePoint Online eller OneDrive for bedrifter fordi en oppbevaringspolicy, oppbevaring etikett eller eDiscovery holder brukes på et SharePoint-område for OneDrive eller et bestemt element. Dette inkluderer at du ikke kan slette et dokument, en dokumentversjon, en mappe, et dokumentbibliotek, en liste, en app, et område eller en områdesamling. Her er noen eksempler på feilmeldinger du kan motta hvis du prøver å slette et element som beholdes:

- "Dette området kan ikke slettes fordi det er inkludert i en eDiscovery holder eller oppbevaringspolicy"
- "Dette området har en samsvars policy som er satt til å blokkere sletting"
- "En samsvars policy blokkerer for øyeblikket slettingen av dette området"
- "Denne områdesamlingen kan ikke slettes fordi den inneholder områder som er inkludert i en eDiscovery holder eller oppbevaringspolicy"
- "Du må slette alle elementene i denne mappen før du sletter mappen"
- "Versjoner av dette elementet kan ikke slettes fordi det er på vent eller oppbevaringspolicy"
- "Elementet kan ikke slettes mens du er på vent"
- "Etiketten som brukes på dette elementet, hindrer den i å redigeres eller slettes"
- "Listen kan ikke slettes når du er på vent eller oppbevaringspolicy"
- "Listen kan ikke slettes hvis den er blokkert, eller hvis en oppbevaringspolicy brukes på den"

For å slette elementer i ett av disse scenariene må oppbevaringspolicyen, oppbevarings etiketten eller eDiscovery-tak fjernes (eller et område må utelates fra en oppbevaringspolicy). Du må enten deaktivere eller ekskludere respektive hold som forårsaker dette problemet. Etter at en oppbevaringspolicy eller et Hold er fjernet, kan det ta opptil 24 timer for endringen trer i kraft. 

Hvis du vil ha informasjon om de forskjellige funksjonene for oppbevaring og hold som kan brukes på SharePoint-områder og OneDrive-kontoer, se ett av følgende emner.

- [Oversikt over oppbevaringspolicyer](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [Oversikt over oppbevarings etiketter](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [Behandle sperringer i avansert eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [eDiscovery inneholder](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [Retningslinjer for avslutning og sletting av eldre områder](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
