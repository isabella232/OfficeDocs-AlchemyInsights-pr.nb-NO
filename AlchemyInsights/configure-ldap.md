---
title: Konfigurere LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885572"
---
# <a name="configure-ldap"></a>Konfigurere LDAP

Gjør følgende for å konfigurere LDAP:

1. Kontroller domenets tilstand på Azure- [portalen](https://aka.ms/aadds-health).
1. Sikre at et gyldig Azure AD-abonnement er tilgjengelig, og at Azure AD Domain Services er aktivert.
1. Sertifikatet som kreves for å tillate sikker LDAP, må hentes fra en klarert offentlig sertifiserings instans eller være et selv signert sertifikat.
1. Pass på at sertifikatet følger de nødvendige [retnings linjene](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Ugyldig sertifikat**
1. Hvis du vil fornye et sertifikat, følger du Fremgangs måten for å opprette et nytt sertifikat og laste det opp på [nytt: Konfigurere LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Hvis du vil løse kjente problemer med sikre LDAP-varsler i Azure Active Directory Domain Services, kan du se [løse LDAP-varsler](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
