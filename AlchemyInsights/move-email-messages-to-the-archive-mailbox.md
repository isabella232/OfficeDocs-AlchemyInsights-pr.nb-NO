---
title: Flytte e-postmeldinger til Arkiv-postboksen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713655"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="0eb96-102">Flytte e-post til arkivpostboksen</span><span class="sxs-lookup"><span data-stu-id="0eb96-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="0eb96-103">Bekreft at en **arkivpostboks** er aktivert.</span><span class="sxs-lookup"><span data-stu-id="0eb96-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="0eb96-104">Hvis ikke, kan du bruke fremgangsmåten i [denne artikkelen](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) til å aktivere arkivpostboksen.</span><span class="sxs-lookup"><span data-stu-id="0eb96-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="0eb96-105">Hvis du vil arkivere meldinger automatisk til arkivpostboksen, må en oppbevaringskode med handlingen **Flytt til arkiv** angis til brukes automatisk på hele **postboksen (standard) koden**.</span><span class="sxs-lookup"><span data-stu-id="0eb96-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="0eb96-106">Bruk fremgangsmåten her for å opprette taggen: [Arkiver standardkoden](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="0eb96-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="0eb96-107">Deretter legger **Archive** du til Arkiv-taggen i oppbevaringspolicyen.</span><span class="sxs-lookup"><span data-stu-id="0eb96-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="0eb96-108">I administrasjonssenteret for Exchange velger du **Oppbevaringspolicyer** > legge **til merket Flytt til arkiv** i policyen > **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="0eb96-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="0eb96-109">Tilordne nå [oppbevaringspolicyen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den bestemte brukerens postboks.</span><span class="sxs-lookup"><span data-stu-id="0eb96-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="0eb96-110">Den samme policyen vil bli brukt på både **primær-** og **arkivpostboksen.**</span><span class="sxs-lookup"><span data-stu-id="0eb96-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="0eb96-111">Det kan være nødvendig å tvinge Administrert mappeassistent (MFA) til å kjøre og bruke de nye innstillingene på brukerens postboks.</span><span class="sxs-lookup"><span data-stu-id="0eb96-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="0eb96-112">Kjør følgende kommando mens [du er koblet til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for å starte administrert mappeassistent for en bestemt postboks:</span><span class="sxs-lookup"><span data-stu-id="0eb96-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="0eb96-113">Start-ManagedFolderAssistant -Identitet<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="0eb96-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="0eb96-114">Hvis du vil ha mer informasjon om hvordan du konfigurerer en arkivpolicy, kan du se [Konfigurere en arkiv- og slettingspolicy for postbokser](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="0eb96-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  