---
title: Et av dine lokale Federation Service Sertifikater utløper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761392"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Et av dine lokale Federation Service Sertifikater utløper

Hvis du vil løse dette problemet, gjør du følgende:
  
- Installer Microsoft Azure Active Directory-modul for Windows PowerShell på datamaskinen (hvis modulen ikke allerede er installert). Hvis du vil gjøre dette, kan du gå til [Azure Active Directory PowerShell for Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Følg trinnene i delen "Scenario 1: AD FS tokensigneringssertifikatet er utløpt" i ["Det oppstod et problem under tilgang til området" fra AD FS når en samlet bruker logger på Office 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Følg trinnene i t[Slik oppdaterer eller reparerer du innstillingene for et forent domene i Office 365, Azure eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Hvis du vil ha mer informasjon om fornyelse av Federation-sertifikater, kan du se [Sertifikatfornyelse for O365 og Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

