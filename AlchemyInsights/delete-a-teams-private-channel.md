---
title: Slette en privat kanal for Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439908"
---
# <a name="delete-a-teams-private-channel"></a>Slette en privat kanal for Teams

Microsoft er klar over et problem med å slette en privat kanal for Teams hvis du har SharePoint-oppbevaringspolicyer aktivert for det underliggende SharePoint-området. Microsoft jobber med en løsning. I mellomtiden kan du bruke følgende løsninger til å slette den private kanalen.

**Utelate gruppe-/områdesamlingen fra sharepoint-oppbevaringspolicyen.**

1. Gå til administrasjonsportalen for Office 365, og velg **Vis alt** i navigasjonsruten til venstre.
2. Gå til **Sikkerhets- &** Policy for hindring av datatap for samsvar under **Administrasjonssentre**  >  **Data Loss Prevention**  >  **Policy**.
3. Identifiser eventuelle policyer som gjelder for Sharepoint-områder, og endre policyen slik at Sharepoint-området for teamet som inneholder den private kanalen, IKKE er inkludert i oppbevaringspolicyen.
4. Lagre retningslinjene.
    Det kan ta opptil 24 timer før policyinnstillingene trer i kraft.
    Når nettstedet er utelukket, kan du slette den private kanalen.  
    
Du ***kan kanskje*** slette den private kanalen ved hjelp av Microsoft Teams på Android-enheten din. 

Hvis du vil ha relatert SharePoint-informasjon, kan du se [Kan ikke slette elementer i SharePoint Online eller OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).