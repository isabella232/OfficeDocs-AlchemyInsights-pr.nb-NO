---
title: Flytte e-postmeldinger til arkivpostboksen automatisk
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
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527105"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="24282-102">Flytte e-postmeldinger til arkivpostboksen automatisk</span><span class="sxs-lookup"><span data-stu-id="24282-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="24282-103">Slik konfigurerer du en policy slik at en brukers gamle e-post flyttes automatisk til arkivpostboksen:</span><span class="sxs-lookup"><span data-stu-id="24282-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="24282-104">Gå til [**Sikkerhet & for**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **samsvarsdatastyringsarkivet** for å bekrefte at en  >   arkivpostboks er aktivert for brukeren.</span><span class="sxs-lookup"><span data-stu-id="24282-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="24282-105">Hvis den ikke har det, klikker du **Aktiver** og **deretter Ja** i advarselen.</span><span class="sxs-lookup"><span data-stu-id="24282-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="24282-106">Gå til [**administrasjonssenteret for Exchange > for samsvarsbehandling > oppbevaringskoder.**](https://go.microsoft.com/fwlink/?linkid=2059104)</span><span class="sxs-lookup"><span data-stu-id="24282-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="24282-107">Velg +-ikonet, og velg **deretter automatisk bruk på hele postboksen.**</span><span class="sxs-lookup"><span data-stu-id="24282-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="24282-108">Tilordne et navn til oppbevaringskoden, og velg **Flytt til arkiv.**</span><span class="sxs-lookup"><span data-stu-id="24282-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="24282-109">Angi ønsket tid for oppbevaringsperioden, for eksempel 90 dager.</span><span class="sxs-lookup"><span data-stu-id="24282-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="24282-110">Klikk på **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="24282-110">Click **Save**.</span></span>
5. <span data-ttu-id="24282-111">Nå kan du opprette en **oppbevaringspolicy: velg** oppbevaringspolicyer, velg ikonet for å legge til en ny policy.</span><span class="sxs-lookup"><span data-stu-id="24282-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="24282-112">Tilordne et navn til oppbevaringspolicyen, og klikk og rull for å finne og legge til oppbevaringskoden du nettopp opprettet.</span><span class="sxs-lookup"><span data-stu-id="24282-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="24282-113">Klikk på **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="24282-113">Click **Save**.</span></span>
7. <span data-ttu-id="24282-114">Til slutt bruker du oppbevaringspolicyen på brukerens postboks: Fortsatt i **administrasjonssenteret** for Exchange, gå til  >  **mottakerpostbokser.**</span><span class="sxs-lookup"><span data-stu-id="24282-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="24282-115">Velg alle brukerne du vil bruke policyen på, og velg deretter **Rediger** (blyantikonet).</span><span class="sxs-lookup"><span data-stu-id="24282-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="24282-116">Klikk postboksfunksjoner i **dialogboksen.**</span><span class="sxs-lookup"><span data-stu-id="24282-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="24282-117">Bruk **policyen du** nettopp opprettet under Oppbevaringspolicy, og > **Lagre.**</span><span class="sxs-lookup"><span data-stu-id="24282-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="24282-118">Hvis du vil ha instruksjoner for hvordan du bruker policyen på alle brukere, kan du se [Bruke en oppbevaringspolicy på postbokser.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="24282-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
