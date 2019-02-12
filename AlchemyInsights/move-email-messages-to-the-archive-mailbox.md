---
title: Flytte e-postmeldinger i postboksen arkiv
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941723"
---
<span data-ttu-id="a0510-p101">Har problemer med arkiveringen elementer til arkiv-postboks. Kontroller at du har utført trinnene nedenfor:</span><span class="sxs-lookup"><span data-stu-id="a0510-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="a0510-p102">Bekreft at en **Arkiver postboks** er aktivert. Hvis ikke, kan du bruke fremgangsmåten i [denne artikkelen](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) til å aktivere arkiv-postboks.</span><span class="sxs-lookup"><span data-stu-id="a0510-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="a0510-106">Opprett en **kode for oppbevaring** med handlingen **Gå til arkiv** som inneholder ønsket **Oppbevaring alder**i Exchange administrasjonssenteret, velg **Oppbevaring koder** under **Behandling av overholdelse**.</span><span class="sxs-lookup"><span data-stu-id="a0510-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="a0510-107">I administrasjonssenteret for Exchange velger **Oppbevaringspolicyer**, opprette en **Oppbevaringspolicy** og legge til din **flytte til** oppbevaring-ID i policyen.</span><span class="sxs-lookup"><span data-stu-id="a0510-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="a0510-p103">[Tilordne oppbevaringspolicyen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til bestemte brukerens postboks. Policyen om samme gjelder både **Primær** og **Arkiv** -postboks.</span><span class="sxs-lookup"><span data-stu-id="a0510-p103">[Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="a0510-p104">Brukerens postboks har nå en arkiveringspolicy til å flytte elementer til arkiv-postboks. Det kan være nødvendig å tvinge den administrerte mappen hjelperen (MFA) til å kjøre og bruke de nye innstillingene i brukerens postboks. Kjør følgende kommando når du [er koblet til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) å starte administrert Mappeassistent for en bestemt postboks:</span><span class="sxs-lookup"><span data-stu-id="a0510-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="a0510-113">Vil ha mer informasjon om hvordan du konfigurerer en arkiveringspolicy for, kan du se [Konfigurere en policy for arkivering og sletting for postbokser](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="a0510-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

