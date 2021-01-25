---
title: Tilordning av attributt for bruker klar gjøring
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949890"
---
# <a name="user-provisioning-attribute-mapping"></a>Tilordning av attributt for bruker klar gjøring

1. Hvis du vil feilsøke kjente problemer med attributtilordning, kan du se [tilordninger av attributter](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings). 
2. Microsoft Azure Active Directory (AD) gir støtte for bruker klar gjøring til tredje parts SaaS-programmer som Salesforce, G Suite og andre. Hvis du aktiverer klar gjøring av bruker for et tredje parts SaaS-program, kontrollerer Azure-portalen de tilhørende attributtverdiene gjennom attributes-tilordninger. Hvis du vil lære hvordan du tilpasser standard attributt tilordninger, kan du se [tilpasse attributtet for klar gjøring av brukere – tilordninger for Saas-programmer i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).
    - Hvis du vil lære mer om klar gjøring av SaaS-apper, kan du se [Hva er automatisert Saas bruker klar gjøring i Azure ad?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Når du tilpasser tilordninger av attributter for bruker klar gjøring, kan det hende at attributtet du vil tilordne, ikke vises i kildeattributtet-listen. [Synkroniser et attributt fra den lokale Active Directory til Azure ad for klar gjøring i en program](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) artikkel viser deg hvordan du legger til det manglende attributtet ved å synkronisere det fra den lokale AD til Azure ad.
