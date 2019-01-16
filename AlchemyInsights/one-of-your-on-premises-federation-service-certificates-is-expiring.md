---
title: Ett av sertifikatene dine lokale Federation Service er utløpt
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 89a4dd910d43d70e849be19d5f88e281f6d19834
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28302679"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Ett av sertifikatene dine lokale Federation Service er utløpt

Hvis du vil løse dette problemet, gjør du følgende:
  
- Installere det Microsoft Azure Active Directory-modulen for Windows PowerShell på datamaskinen (Hvis modulen ikke er allerede installert). Hvis du vil gjøre dette, kan du gå til [Azure Active Directory PowerShell for diagram](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Følg trinnene i den "Scenario 1: AD FS token signere sertifikatet er utløpt" delen av ["Det oppstod en feil under tilgang til området" feil fra AD FS når en forent bruker logger på Office 365, Azure, eller Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Følg trinnene i t[hvordan å oppdatere eller reparere innstillingene for medlemmer av organisasjonsnettverk domene i Office 365, Azure, eller Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Hvis du vil ha mer informasjon om å fornye Federation sertifikater, kan du se [sertifikatfornyelse for O365 og Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

