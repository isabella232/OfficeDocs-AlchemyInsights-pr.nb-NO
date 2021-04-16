---
title: Et av de lokale forbundstjenestesertifikatene utløper
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810061"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Et av de lokale forbundstjenestesertifikatene utløper

Følg disse trinnene for å løse dette problemet:
  
- Installer Microsoft Azure Active Directory-modulen for Windows PowerShell på datamaskinen (hvis modulen ikke allerede er installert). Dette gjør du ved å gå til [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Følg fremgangsmåten i avsnittet «Scenario 1: AD FS token-signeringssertifikatet er utløpt» i feilmeldingen «Det oppstod et problem med tilgang til nettstedet» fra AD FS når en bruker i forbund logger på [Microsoft 365, Azure eller Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)
    
- Følg fremgangsmåten i Slik oppdaterer eller reparerer du innstillingene for et domene i forbund i [Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Hvis du vil ha mer informasjon om fornyelse av forbundssertifikater, kan du se [Sertifikatfornyelse for O365 og Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

