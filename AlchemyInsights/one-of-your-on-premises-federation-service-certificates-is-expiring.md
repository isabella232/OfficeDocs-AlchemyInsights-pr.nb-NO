---
title: Et av de lokale Forbunds tjeneste sertifikatene utløper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673506"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Et av de lokale Forbunds tjeneste sertifikatene utløper

Følg denne Fremgangs måten for å løse dette problemet:
  
- Installer Microsoft Azure Active Directory-modulen for Windows PowerShell på data maskinen (Hvis modulen ikke allerede er installert). Hvis du vil gjøre dette, går du til [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Følg Fremgangs måten i delen "scenario 1: signerings sertifikatet for AD FS token utløpt" i [«det oppstod et problem under tilgang til nettstedet» fra AD FS når en Forbunds bruker logger seg på Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- Følg trinnene i [hvordan du oppdaterer eller reparerer innstillingene for et organisasjons nettverk i Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Hvis du vil ha mer informasjon om hvordan du fornyer forbundede sertifikater, kan du se [sertifikat fornyelse for O365 og Azure ad](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

