---
title: ADFS Federation sertifikat utløper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710416"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federation sertifikat utløper

Hvis du vil løse dette problemet, gjør du følgende:
  
1. Installer Microsoft Azure Active Directory-modul for Windows PowerShell på datamaskinen (hvis modulen ikke allerede er installert). Hvis du vil gjøre dette, kan du gå til [Administrere Azure AD ved hjelp av Windows PowerShell](https://aka.ms/aadposh).

2. Følg trinnene i delen "Scenario 1: AD FS tokensigneringssertifikatet er utløpt" i ["Det oppstod et problem under tilgang til området" fra AD FS når en samlet bruker logger på Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Følg trinnene i [Oppdatere eller reparere innstillingene for et forent domene i Microsoft, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Hvis du vil vite mer om fornyelse av Federation-sertifikater, kan du se [Fornye federation sertifikater for Microsoft 365 og Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
