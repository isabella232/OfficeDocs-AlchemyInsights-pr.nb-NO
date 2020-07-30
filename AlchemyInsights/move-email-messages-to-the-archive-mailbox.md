---
title: Flytte e-postmeldinger til arkivpostboksen
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
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522780"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="e3a35-102">Flytte e-post til arkivpostboksen</span><span class="sxs-lookup"><span data-stu-id="e3a35-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="e3a35-103">Hvis du vil at vi skal kjøre automatiserte kontroller for innstillingene nevnt nedenfor, velger du tilbakeknappen < - øverst på denne siden, og deretter skriver du inn e-postadressen til brukeren som har problemer med å flytte e-post til arkivpostboksen.</span><span class="sxs-lookup"><span data-stu-id="e3a35-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="e3a35-104">Kontroller at en **arkivpostboks** er aktivert.</span><span class="sxs-lookup"><span data-stu-id="e3a35-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="e3a35-105">Hvis ikke, kan du bruke fremgangsmåten i [denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) til å aktivere arkivpostboksen.</span><span class="sxs-lookup"><span data-stu-id="e3a35-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="e3a35-106">Hvis du vil arkivere meldinger automatisk til arkivpostboksen, må en oppbevaringskode med handlingen **Flytt til arkiv** settes til å brukes automatisk på hele **postbokskoden (standard).**</span><span class="sxs-lookup"><span data-stu-id="e3a35-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="e3a35-107">Bruk fremgangsmåten her for å opprette koden: [Arkiver standardkode](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="e3a35-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="e3a35-108">Deretter legger **Archive** du til Arkiv-taggen i oppbevaringspolicyen.</span><span class="sxs-lookup"><span data-stu-id="e3a35-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="e3a35-109">I administrasjonssenteret for Exchange velger du **Oppbevaringspolicyer** > legge **til flytt til arkiv-koden** i policyen > **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="e3a35-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="e3a35-110">Tilordne [nå oppbevaringspolicyen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den bestemte brukerens postboks.</span><span class="sxs-lookup"><span data-stu-id="e3a35-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="e3a35-111">Den samme policyen brukes på både **primær-** og **arkivpostboksen.**</span><span class="sxs-lookup"><span data-stu-id="e3a35-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="e3a35-112">Det kan være nødvendig å tvinge administrertmappeassistent (MFA) til å kjøre og bruke de nye innstillingene på brukerens postboks.</span><span class="sxs-lookup"><span data-stu-id="e3a35-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="e3a35-113">Kjør følgende kommando mens [du er koblet til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for å starte administrertmappeassistent for en bestemt postboks:</span><span class="sxs-lookup"><span data-stu-id="e3a35-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="e3a35-114">Start-ManagedFolderAssistant -Identitet<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="e3a35-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="e3a35-115">Hvis du vil ha mer informasjon om hvordan du konfigurerer en arkivpolicy, kan du se [Definere en policy for arkivering og sletting for postbokser](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="e3a35-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  