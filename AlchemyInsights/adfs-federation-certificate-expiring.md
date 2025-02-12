---
title: ADFS-forbundssertifikat utløper
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
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952978"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS-forbundssertifikat utløper

Følg disse trinnene for å løse dette problemet:
  
1. Installer Microsoft Azure Active Directory-modulen for Windows PowerShell på datamaskinen (hvis modulen ikke allerede er installert). Dette gjør du ved å gå til [Administrere Azure AD ved hjelp av Windows PowerShell](https://aka.ms/aadposh).

2. Følg fremgangsmåten i avsnittet «Scenario 1: AD FS token-signeringssertifikatet er utløpt» i feilmeldingen «Det oppstod et problem med tilgang til nettstedet» fra AD FS når en bruker i forbund logger på Microsoft 365, Azure eller [Intune.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Følg fremgangsmåten i Oppdatere eller reparere innstillingene for et domene i forbund [i Microsoft, Azure eller Intune.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Hvis du vil lære mer om fornyelse av forbundssertifikater, kan du se Fornye [forbundssertifikater for](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)Microsoft 365 og Azure Active Directory .
