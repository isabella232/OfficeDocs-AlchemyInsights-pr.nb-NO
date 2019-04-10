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
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747212"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="83f47-102">Flytt e-post til arkiv-postboks</span><span class="sxs-lookup"><span data-stu-id="83f47-102">Move email to the archive mailbox</span></span>
 
1. <span data-ttu-id="83f47-103">Bekreft at en **Arkiver postboks** er aktivert.</span><span class="sxs-lookup"><span data-stu-id="83f47-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="83f47-104">Hvis ikke, Bruk fremgangsmåten i [denne artikkelen](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) for å aktivere arkiv-postboks.</span><span class="sxs-lookup"><span data-stu-id="83f47-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="83f47-105">En oppbevaring kode med handlingen **flytter å arkivere** må være satt til **automatisk gjelder hele postboksen (standard)-kode**for å arkivere meldinger automatisk til arkiv-postboks.</span><span class="sxs-lookup"><span data-stu-id="83f47-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="83f47-106">Bruk fremgangsmåten her for å opprette merket: [Arkiv standard kode](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span><span class="sxs-lookup"><span data-stu-id="83f47-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>
    
3. <span data-ttu-id="83f47-107">Deretter legge til **Arkiv** -koden din oppbevaringspolicy.</span><span class="sxs-lookup"><span data-stu-id="83f47-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="83f47-108">Velg **Oppbevaringspolicyer** i Exchange-administrasjonssenteret > legge til **Flytt til arkiv kode** policy-> **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="83f47-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span> 
    
4. <span data-ttu-id="83f47-109">Nå [tilordne oppbevaringspolicyen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til bestemte brukerens postboks.</span><span class="sxs-lookup"><span data-stu-id="83f47-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="83f47-110">Policyen om samme gjelder både **Primær** og **Arkiv** -postboks.</span><span class="sxs-lookup"><span data-stu-id="83f47-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="83f47-111">Det kan være nødvendig å tvinge den administrerte mappen hjelperen (MFA) til å kjøre og bruke de nye innstillingene i brukerens postboks.</span><span class="sxs-lookup"><span data-stu-id="83f47-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="83f47-112">Kjør følgende kommando når du [er koblet til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) å starte administrert Mappeassistent for en bestemt postboks:</span><span class="sxs-lookup"><span data-stu-id="83f47-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="83f47-113">Hvis du vil ha mer informasjon om hvordan du konfigurerer en arkiveringspolicy, kan du se [Konfigurere en policy for arkivering og sletting for postbokser](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="83f47-113">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

