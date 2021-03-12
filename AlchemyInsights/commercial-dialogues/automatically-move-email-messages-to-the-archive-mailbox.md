---
title: Flytte e-postmeldinger automatisk til arkivpostboksen
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749283"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="e9bd1-102">Flytte e-postmeldinger automatisk til arkivpostboksen</span><span class="sxs-lookup"><span data-stu-id="e9bd1-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="e9bd1-103">Slik konfigurerer du en policy for automatisk å flytte en brukers gamle e-post til arkivpostboksen:</span><span class="sxs-lookup"><span data-stu-id="e9bd1-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="e9bd1-104">Gå til [**Arkiv for & for**](https://go.microsoft.com/fwlink/p/?linkid=2077143)samsvarsdata for å bekrefte at en arkivpostboks er aktivert for  >    >   brukeren.</span><span class="sxs-lookup"><span data-stu-id="e9bd1-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="e9bd1-105">Hvis den ikke har det, klikker du **aktiver** deretter **Ja** i advarselsboksen.</span><span class="sxs-lookup"><span data-stu-id="e9bd1-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="e9bd1-106">Gå til [**Administrasjonssenter for Exchange > samsvarsbehandling > oppbevaringskoder**](https://go.microsoft.com/fwlink/?linkid=2059104).</span><span class="sxs-lookup"><span data-stu-id="e9bd1-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="e9bd1-107">Velg +-ikonet, og **velg deretter automatisk bruk på hele postboksen**.</span><span class="sxs-lookup"><span data-stu-id="e9bd1-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="e9bd1-108">Tilordne et navn til oppbevaringskoden, og velg **Flytt til arkiv**.</span><span class="sxs-lookup"><span data-stu-id="e9bd1-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="e9bd1-109">Angi ønsket tidspunkt for oppbevaringsperioden, for eksempel 90 dager.</span><span class="sxs-lookup"><span data-stu-id="e9bd1-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="e9bd1-110">Klikk på **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="e9bd1-110">Click **Save**.</span></span>
5. <span data-ttu-id="e9bd1-111">Opprett nå en oppbevaringspolicy: Velg **oppbevaringspolicyer**, velg ikonet for å legge til en ny policy.</span><span class="sxs-lookup"><span data-stu-id="e9bd1-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="e9bd1-112">Tilordne et navn til oppbevaringspolicyen, og klikk og rull for å finne og legge til oppbevaringskoden du nettopp opprettet.</span><span class="sxs-lookup"><span data-stu-id="e9bd1-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="e9bd1-113">Klikk på **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="e9bd1-113">Click **Save**.</span></span>
7. <span data-ttu-id="e9bd1-114">Til slutt bruker du oppbevaringspolicyen på brukerens postboks: Fortsatt i **administrasjonssenteret** for Exchange går du til  >  **mottakerpostbokser**.</span><span class="sxs-lookup"><span data-stu-id="e9bd1-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="e9bd1-115">Velg alle brukerne du vil bruke policyen på, og velg deretter **Rediger** (blyantikonet).</span><span class="sxs-lookup"><span data-stu-id="e9bd1-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="e9bd1-116">Klikk postboksfunksjoner i **dialogboksen**.</span><span class="sxs-lookup"><span data-stu-id="e9bd1-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="e9bd1-117">Under **Oppbevaringspolicy** bruker du policyen du nettopp opprettet > **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="e9bd1-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="e9bd1-118">Hvis du vil ha instruksjoner for hvordan du bruker policyen for alle brukere, kan du se [Bruke en oppbevaringspolicy på postbokser](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span><span class="sxs-lookup"><span data-stu-id="e9bd1-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
