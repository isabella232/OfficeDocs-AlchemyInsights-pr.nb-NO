---
title: Skrivebeskyttet for vedlikehold melding når du prøver å bruke SharePoint- eller OneDrive
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620732"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Skrivebeskyttet for vedlikehold melding når du prøver å bruke SharePoint- eller OneDrive

Brukere kan få en **Skrivebeskyttet for vedlikehold** melding når du prøver å bruke SharePoint- eller OneDrive for ett av følgende scenarier. 

-   En aktivitet planlagt eller aktiv vedlikehold.  Se etter dem ved å navigere til [Meldingssentral](https://portal.office.com/adminportal/home#/messagecenter).
-   En høy prioritet, aktive tjenesten problemer som kan oppstå. Se etter eventuelle veiledningene/hendelser ved å navigere til [Health Service](https://portal.office.com/adminportal/home#/servicehealth).
-   Et mindre automatisk reparasjon gjenoppretting scenario som kan skje på grunn av uventede hendelser på servere som kan vare i mindre enn 30 minutter eller så. 
    
    Det finnes ingen Message Center eller tjenesten helse bokfører disse underordnede gjenopprettinger, men du bør være tilbake til normal veldig snart.

Vi observerte at én av tre scenariene ovenfor er årsaken, og tjenesten er gjenopprettet, men hurtigbufferen for webleseren brukere ikke har blitt tømt i svært få tilfeller.

Prøv å tømme hurtigbufferen for webleseren før du navigere til området.

1. I webleseren Microsoft Edge, velg **Innstillinger**, og velg deretter **Personvern og sikkerhet**.
2. **Fjern Bla gjennom**, velg **Velg hva du vil fjerne**.
3. Velg **informasjonskapsler og webområdet for lagrede data**, og velg **Fjern**.

>[!Note] 
> Disse trinnene kan variere når du bruker andre lesere, for eksempel Mozilla Firefox eller Google Chrome.

>[!Note] 
> Et annet alternativ er å åpne SharePoint-området eller OneDrive i et nytt InPrivate-vindu.