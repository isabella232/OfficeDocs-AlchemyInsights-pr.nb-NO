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
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090421"
---
# <a name="configure-ldap"></a>Konfigurere LDAP

Gjør følgende for å konfigurere LDAP:

1. Kontroller domenets tilstand på [Azure-portalen.](https://aka.ms/aadds-health)
1. Kontroller at et gyldig Azure AD-abonnement er tilgjengelig, og at Azure AD Domain Services er aktivert.
1. Sertifikatet som kreves for å aktivere sikker LDAP, må hentes fra en klarert offentlig sertifiseringsinstans eller være et selvsignert sertifikat.
1. Kontroller at sertifikatet følger de nødvendige [retningslinjene](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).

**Ugyldig sertifikat**
1. Hvis du vil fornye et sertifikat, følger du fremgangsmåten for å opprette et nytt sertifikat og laste inn på [nytt: Konfigurere LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
1. Hvis du vil løse kjente problemer med Secure LDAP-varsler i Azure Active Directory Domain Services, kan du se [Løse LDAP-varsler](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).
