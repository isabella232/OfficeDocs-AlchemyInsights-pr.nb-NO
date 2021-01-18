---
title: Virtuell konfigurasjon med AAD Domain Services
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885644"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuell konfigurasjon med AAD Domain Services

Virtuell konfigurasjon med AAD Domain Services omfatter følgende trinn: 

1. Kontrollere domenets tilstand på Azure-portalen https://aka.ms/aadds-health
2. Kontrollere NSG for regler som blokkerer porter som er nødvendige for å synkronisere i Azure AD Domain Services på portalen https://aka.ms/aadds-networking
3. Sørge for at det virtuelle nettverket er distribuert i samme Azure-område som Azure AD Domain Services-administrert domene.
4. Sikre at du ikke har et eksisterende domene med samme domene navn som er tilgjengelig på det virtuelle nettverket.

Hvis du vil ha mer informasjon om utformings hensyn for Azure virtuelt nettverk for å støtte AAD Domain Services, kan du se [virtuelt nettverks vurdering](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

