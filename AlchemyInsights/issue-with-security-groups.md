---
title: Problem med sikkerhetsgrupper
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177628"
---
# <a name="issue-with-security-groups"></a>Problem med sikkerhetsgrupper

**Hvis du får nettverksfeil AADDS104**

Ugyldige grupperegler for nettverkssikkerhet er den vanligste årsaken til nettverksfeil for Azure Active Directory Domain Services (AD DS). Sikkerhetsgruppen for nettverket for det virtuelle nettverket må tillate tilgang til bestemte porter og protokoller. Hvis disse portene er blokkert, kan ikke Azure-plattformen overvåke eller oppdatere det administrerte domenet. Synkroniseringen mellom Azure AD og Azure AD DS påvirkes også. Sørg for at standardportene er åpne for å unngå avbrudd i tjenesten.

Hvis du vil forstå og løse vanlige varsler om konfigurasjonsproblemer for nettverkssikkerhetsgrupper, kan du se [Legge til og bekrefte sikkerhetsgrupper.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)
