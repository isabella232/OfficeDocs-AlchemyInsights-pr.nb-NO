---
title: Skrivebeskyttet for vedlikeholds melding når du prøver å bruke SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670841"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Skrivebeskyttet for vedlikeholds melding når du prøver å bruke SharePoint eller OneDrive

Brukere kan motta en **skrivebeskyttet for vedlikeholds** melding når du prøver å bruke SharePoint eller OneDrive for ett av følgende scenarioer. 

-   En planlagt eller aktiv vedlikeholds aktivitet.  Se etter dem ved å navigere til [meldings senteret](https://portal.office.com/adminportal/home#/messagecenter).
-   En aktiv tjeneste hendelse med høy prioritet, som kan oppstå. Se etter en rådgiver/hendelser ved å navigere til [tjeneste tilstand](https://portal.office.com/adminportal/home#/servicehealth).
-   Et mindre scenario for automatisk reparasjons gjenoppretting som kan oppstå på grunn av eventuelle uventede hendelser på serverne som kanskje har mindre enn 30 min eller så videre. 
    
    Det finnes ingen inn Legg for meldings senter eller tjeneste tilstander for disse underordnede oppmøtene, men du bør snart gå tilbake til normal.

I svært få tilfeller observerte vi at et av de tre scenariene som er oppført ovenfor, har vært årsaken, og at tjenesten er gjen opprettet, men brukernes nett leser buffer er ikke tømt.

Prøv å tømme nett leser bufferen før du navigerer til området.

1. Velg **Innstillinger**i Microsoft Edge-leseren, og velg deretter **person vern og sikkerhet**.
2. Under **Tøm nett lesing**velger **du Velg hva som skal fjernes**.
3. Velg **informasjons kapsler og lagrede nettsteds data**, og velg **Fjern**.

>[!Note] 
> Disse trinnene kan variere når du bruker andre nett lesere, for eksempel Mozilla Firefox eller Google Chrome.

>[!Note] 
> Et annet alternativ vil være å åpne SharePoint-området eller OneDrive i et nytt InPrivate-vindu.