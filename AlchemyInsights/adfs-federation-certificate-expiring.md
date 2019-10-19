---
title: ADFS Federation sertifikat utløper
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737198"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federation sertifikat utløper

Hvis du vil løse dette problemet, følger du denne fremgangsmåten:
  
1. Installere Microsoft Azure Active Directory-modul for Windows PowerShell på datamaskinen (Hvis modulen ikke allerede er installert). Hvis du vil gjøre dette, kan du gå til [Administrer Azure ad ved hjelp av Windows PowerShell](https://aka.ms/aadposh).

2. Følg trinnene i den "scenario 1: AD FS token signeringssertifikatet er utløpt" delen av ["det oppstod et problem under tilgang til området" feil fra AD FS når en forent bruker logger på Office 365, Azure eller Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Følg trinnene i [oppdatere eller reparere innstillingene for et forent domene i Office 365, Azure eller Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    Hvis du vil ha mer informasjon om fornyelse av Federation sertifikater, kan du se [fornye Federation sertifikater for Office 365 og Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
