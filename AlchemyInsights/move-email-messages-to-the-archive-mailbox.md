---
title: Flytt e-postmeldinger til arkiv-postkassen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822171"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="00775-102">Flytt e-post til arkivpostboksen</span><span class="sxs-lookup"><span data-stu-id="00775-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="00775-103">Kontroller at en **arkivpostboks** er aktivert.</span><span class="sxs-lookup"><span data-stu-id="00775-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="00775-104">Hvis ikke, bruker du fremgangsmåten i [denne artikkelen](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) til å aktivere arkiv-postboksen.</span><span class="sxs-lookup"><span data-stu-id="00775-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="00775-105">Hvis du vil arkivere meldinger automatisk til arkivpostboksen, må en oppbevaringskode med **Flytt til arkiv** -handlingen settes til å **brukes automatisk på hele postboks koden (standard)**.</span><span class="sxs-lookup"><span data-stu-id="00775-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="00775-106">Bruk fremgangsmåten her for å opprette taggen: [Arkiver standardkode](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="00775-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="00775-107">Deretter legger du til **arkiv** koden i oppbevaringspolicyen.</span><span class="sxs-lookup"><span data-stu-id="00775-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="00775-108">I administrasjonssenteret for Exchange velger du **oppbevaringspolicyer** > legger til **Flytt til arkiv-koden** i policyen > **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="00775-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="00775-109">Nå kan du [Tilordne oppbevaringspolicyen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den bestemte brukerens postboks.</span><span class="sxs-lookup"><span data-stu-id="00775-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="00775-110">Den samme policyen vil bli brukt både på **Primær** -og **arkiv** postboksen.</span><span class="sxs-lookup"><span data-stu-id="00775-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="00775-111">Det kan være nødvendig å tvinge administrert Mappeassistent (MFA) til å kjøre og bruke de nye innstillingene til brukerens postboks.</span><span class="sxs-lookup"><span data-stu-id="00775-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="00775-112">Kjør følgende kommando mens du er [koblet til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) til å starte assistenten for administrerte mapper for en bestemt postboks:</span><span class="sxs-lookup"><span data-stu-id="00775-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="00775-113">Start-ManagedFolderAssistant-identitet<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="00775-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="00775-114">Hvis du vil ha mer informasjon om hvordan du konfigurerer en arkiveringspolicy, kan du se [konfigurere en arkiverings-og slettings policy for postbokser](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="00775-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  