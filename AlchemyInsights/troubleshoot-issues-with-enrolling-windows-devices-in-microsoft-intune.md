---
title: Feilsøke problemer med registrering av Windows-enheter i Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661562"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Feilsøke problemer med registrering av Windows-enheter i Microsoft Intune

Se gjennom ressursene som vises nedenfor for å løse problemet nå. 
  
Noen vanlige feilmeldinger og Løsningstrinn:
  
 **Kan ikke installere programvaren, 0x80cf4017:** Konto-sertifikatet er utløpt. Nytt Last ned PC-klient programvaren i Intune Admin-konsollen. Se dokumentasjonen for mer informasjon. 
  
 **0x801c0003-feilkode:** Feilen kan oppstå i følgende scenarier: 
  
1. Brukeren har flere enheter som er registrert enn enhetsgrensen. Se gjennom disse dokumentene for å [fjerne en enhet](https://docs.microsoft.com/intune/devices-wipe) , eller [Endre begrensningen for enheten](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Brukere kan koble enheter til Azure AD" er satt til "ingen". Sett den til alle, eller Velg brukere. Gå gjennom [denne dokumentasjonen](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for mer informasjon. 
    
3. Enheten er allerede registrert av en annen bruker. Hvis det er tilfellet, fjerner du enheten fra konsollen Azure Intune eller unenroll enheten manuelt før du prøver på nytt.
    
4. Enheten er Windows Home 10. Bare Windows 10 Pro, utdanning og Enterprise SKUer kan delta Azure Active Directory.
    
Ytterligere ressurser til å løse problemet:
  
1. Bruke [Intune feilsøking Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) til å diagnostisere og løse vanlige registrering-feil. Gå gjennom [dette dokumentet](https://docs.microsoft.com/intune/help-desk-operators) for mer informasjon. 
    
2. Se gjennom disse dokumentene for en liste over vanlige feil som hindrer registrering og løsninger for hver: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) og [feilsøking dok](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Lær hvordan du kan registrere Windows-enheter i Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
  

