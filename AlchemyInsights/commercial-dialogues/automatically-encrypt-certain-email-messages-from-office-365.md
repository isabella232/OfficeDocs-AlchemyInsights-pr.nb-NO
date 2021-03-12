---
title: Kryptere bestemte e-postmeldinger automatisk fra Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749462"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="79d18-102">Kryptere bestemte e-postmeldinger automatisk fra Office 365</span><span class="sxs-lookup"><span data-stu-id="79d18-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="79d18-103">Velg [e-postflyt i](https://outlook.office365.com/ecp/) **administrasjonssenteret for** Exchange > regler .</span><span class="sxs-lookup"><span data-stu-id="79d18-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="79d18-104">Klikk på **Nytt (+)-ikonet,** og klikk deretter Bruk Meldingskryptering og rettighetsbeskyttelse for **Office 365 på meldinger.**</span><span class="sxs-lookup"><span data-stu-id="79d18-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="79d18-105">Skriv **inn** et navn på regelen i Navn , for eksempel *Krypter alle meldinger*.</span><span class="sxs-lookup"><span data-stu-id="79d18-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="79d18-106">I **Bruk denne regelen hvis** velger du **[Bruk på alle meldinger]**.</span><span class="sxs-lookup"><span data-stu-id="79d18-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="79d18-107">Klikk Velg et ved siden **av** Gjør **følgende-feltet.**</span><span class="sxs-lookup"><span data-stu-id="79d18-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="79d18-108">Velg Krypter på rullegardinmenyen for **RMS-malen,** og klikk deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="79d18-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="79d18-109">(Hvis du ikke ser dette alternativet, betyr det at planen ikke inkluderer automatisk kryptering.</span><span class="sxs-lookup"><span data-stu-id="79d18-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="79d18-110">Men du kan legge den til!)</span><span class="sxs-lookup"><span data-stu-id="79d18-110">But you can add it!)</span></span>
7. <span data-ttu-id="79d18-111">Merk av **for Overvåk denne** regelen med alvorsgrad, og velg deretter ønsket nivå.</span><span class="sxs-lookup"><span data-stu-id="79d18-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="79d18-112">Hvis firmaet har kontraktsmessige forpliktelser til å sende alle e-postmeldinger kryptert, anbefaler jeg å sette nivået til **Høy**.</span><span class="sxs-lookup"><span data-stu-id="79d18-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="79d18-113">Klikk **Påtving under** Velg en modell for denne **regelen.**</span><span class="sxs-lookup"><span data-stu-id="79d18-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="79d18-114">Velg et valgfritt utvalg (fra en liste over valgfrie valg som du kan gjøre på dette tidspunktet, hvorav mange kan stå igjen med standardinnstillingen for enkelhet).</span><span class="sxs-lookup"><span data-stu-id="79d18-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="79d18-115">Klikk på **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="79d18-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="79d18-116">Du kan alltid komme tilbake og redigere denne regelen senere.</span><span class="sxs-lookup"><span data-stu-id="79d18-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="79d18-117">Hvis du vil ha mer informasjon om hvordan du oppretter regler for kryptering, kan du se Definere regler for e-postflyt for [å kryptere e-postmeldinger i Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="79d18-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

