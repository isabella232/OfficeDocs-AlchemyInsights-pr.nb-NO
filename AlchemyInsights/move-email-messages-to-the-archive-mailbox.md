---
title: Flytte e-postmeldinger til arkiv post boksen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799789"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="c0cad-102">Flytte e-post til arkiv post boksen</span><span class="sxs-lookup"><span data-stu-id="c0cad-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="c0cad-103">Hvis du vil at vi skal kjøre automatiske kontroller for innstillingene som nevnes nedenfor, velger du tilbake-knappen < øverst på siden, og deretter skriver du inn e-postadressen til brukeren som har problemer med å flytte e-post til arkiv post boksen.</span><span class="sxs-lookup"><span data-stu-id="c0cad-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="c0cad-104">Kontroller at en **arkiv post boks** er aktivert.</span><span class="sxs-lookup"><span data-stu-id="c0cad-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="c0cad-105">Hvis ikke, bruker du Fremgangs måten i [denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) til å aktivere arkiv post boksen.</span><span class="sxs-lookup"><span data-stu-id="c0cad-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="c0cad-106">Hvis du vil arkivere meldinger automatisk til arkiv post boksen, må en oppbevarings kode med handlingen **Flytt til arkiv** være satt til **automatisk å brukes for hele post boks koden (standard)**.</span><span class="sxs-lookup"><span data-stu-id="c0cad-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="c0cad-107">Bruk Fremgangs måten nedenfor for å opprette koden: [Arkiver standard-kode](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="c0cad-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="c0cad-108">Deretter legger du til **arkiv** koden i oppbevarings policyen.</span><span class="sxs-lookup"><span data-stu-id="c0cad-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="c0cad-109">I administrasjons senteret for Exchange velger du **oppbevarings policyer** for > legge til **Flytt til arkiv-koden** i policyen > **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="c0cad-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="c0cad-110">Nå kan du [Tilordne oppbevarings policyen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) til den bestemte brukerens post boks.</span><span class="sxs-lookup"><span data-stu-id="c0cad-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="c0cad-111">Den samme policyen vil bli brukt på både **Primær** -og **arkiv** post boksen.</span><span class="sxs-lookup"><span data-stu-id="c0cad-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="c0cad-112">Det kan være nødvendig å tvinge gjennom MFA (Managed folder Assistant) for å kjøre og bruke de nye innstillingene på brukerens post boks.</span><span class="sxs-lookup"><span data-stu-id="c0cad-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="c0cad-113">Kjør følgende kommando mens du er [koblet til EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) for å starte den forvaltede mappe assistenten for en bestemt post boks:</span><span class="sxs-lookup"><span data-stu-id="c0cad-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="c0cad-114">Start-ManagedFolderAssistant-identitet <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="c0cad-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="c0cad-115">Hvis du vil ha mer informasjon om hvordan du konfigurerer en arkiv policy, kan du se [konfigurere en policy for arkivering og sletting for post bokser](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="c0cad-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  