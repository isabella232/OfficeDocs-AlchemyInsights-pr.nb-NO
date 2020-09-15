---
title: Sertifikat utløp for ADFS-forbund
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686754"
---
# <a name="adfs-federation-certificate-expiring"></a>Sertifikat utløp for ADFS-forbund

Følg denne Fremgangs måten for å løse dette problemet:
  
1. Installer Microsoft Azure Active Directory-modulen for Windows PowerShell på data maskinen (Hvis modulen ikke allerede er installert). Hvis du vil gjøre dette, går du til [administrere Azure ad ved hjelp av Windows PowerShell](https://aka.ms/aadposh).

2. Følg Fremgangs måten i delen "scenario 1: signerings sertifikatet for AD FS token utløpt" i [«det oppstod et problem under tilgang til nettstedet» fra AD FS når en Forbunds bruker logger seg på Microsoft 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Følg trinnene i [oppdatere eller reparere innstillingene for et organisasjons domene i Microsoft, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Hvis du vil vite mer om hvordan du fornyer forbundede sertifikater, kan du se [fornye forbundede sertifikater for Microsoft 365 og Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
