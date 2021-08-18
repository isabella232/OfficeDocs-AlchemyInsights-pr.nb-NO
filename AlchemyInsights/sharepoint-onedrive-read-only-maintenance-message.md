---
title: Read-Only for vedlikeholdsmelding når du prøver å bruke SharePoint eller OneDrive
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
ms.openlocfilehash: 376b653b18857103586e25edd0ad6801a7bbe0a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329457"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>Read-Only for vedlikeholdsmelding når du prøver å bruke SharePoint eller OneDrive

Brukere kan motta **en skrivebeskyttet for** vedlikeholdsmelding når de prøver å bruke SharePoint eller OneDrive for ett av følgende scenarier. 

-   En planlagt eller aktiv vedlikeholdsaktivitet.  Se etter dem ved å gå til [meldingssenteret](https://portal.office.com/adminportal/home#/messagecenter).
-   En aktiv tjenestehendelse med høy prioritet som kan oppstå. Se etter veiledninger/hendelser ved å gå til [Tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).
-   Et mindre scenario for gjenoppretting av automatisk gjenoppretting som kan skje på grunn av uventede hendelser på serverne som kan vare i mindre enn 30 minutter eller så. 
    
    Det finnes ingen innlegg om meldingssenter eller tjenestetilstand for disse mindre gjenopprettingene, men du bør være tilbake til normalen ganske snart.

I svært få tilfeller observerte vi at ett av de tre scenariene som er oppført ovenfor, har vært årsaken, og at tjenesten har blitt gjenopprettet, men hurtigbufferen for brukernes nettleser har ikke blitt tømt.

Prøv å tømme hurtigbufferen for nettleseren før du navigerer til nettstedet.

1. Velg Microsoft Edge i nettleseren, **Innstillinger**, og velg deretter **Personvern og sikkerhet**.
2. Velg **Velg hva du** vil fjerne, under Fjern **nettlesing**.
3. Velg **Informasjonskapsler og lagrede nettstedsdata**, og velg **Fjern**.

**Obs!** Disse trinnene kan variere når du bruker andre nettlesere, for eksempel Mozilla Firefox eller Google Chrome.

**Obs!** Et annet alternativ er å åpne SharePoint eller OneDrive i et nytt InPrivate-vindu.