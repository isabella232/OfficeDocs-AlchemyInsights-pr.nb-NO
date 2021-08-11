---
title: Test IRM-konfigurasjon for nye OME-funksjoner
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812441"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>Test IRM-konfigurasjon for nye OME-funksjoner

Hvis du vil kontrollere at Microsoft 365-tenanten er konfigurert til å bruke nye OME-funksjoner, kjører du følgende cmdleter mens du er koblet til [Exchange Online PowerShell:](/powershell/exchange/exchange-online-powershell)


1. Kontroller tenantens IRM-konfigurasjon ved å kjøre `Get-IRMConfiguration` . Kontroller at disse verdiene er satt til **Sann:**
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. Bruk domenet, avsenderadressen og mottakeren til å kjøre `Test-IRMConfiguration` . Hvis testen ikke består, undersøker du IRM-konfigurasjonen.

Hvis du vil ha mer informasjon om hvordan du kontrollerer IRM-konfigurasjonen, kan du se Bekrefte ny [OME-konfigurasjon i Exchange Online PowerShell](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).