---
title: Kryptere Office 365-e-postmeldinger som sendes til bestemte domener automatisk
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526692"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="e15df-102">Kryptere Office 365-e-postmeldinger som sendes til bestemte domener automatisk</span><span class="sxs-lookup"><span data-stu-id="e15df-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="e15df-103">Velg [e-postflyt i](https://outlook.office365.com/ecp/)administrasjonssenteret for Exchange, og **> reglene.**</span><span class="sxs-lookup"><span data-stu-id="e15df-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="e15df-104">Klikk på **Nytt (+)-ikonet,** og klikk deretter på Bruk **Office 365-meldingskryptering og rettighetsbeskyttelse på meldinger.**</span><span class="sxs-lookup"><span data-stu-id="e15df-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="e15df-105">Skriv **inn** et navn på regelen i Navn, for eksempel Krypter *meldinger som sendes til contoso.com.*</span><span class="sxs-lookup"><span data-stu-id="e15df-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="e15df-106">I **Bruk denne regelen hvis** velger du mottakeren > domenet **er.**</span><span class="sxs-lookup"><span data-stu-id="e15df-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="e15df-107">Skriv inn navnet på domenet, for eksempel **contoso.com.**</span><span class="sxs-lookup"><span data-stu-id="e15df-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="e15df-108">Klikk legg **til (+)-ikonet,** og klikk deretter **OK.**</span><span class="sxs-lookup"><span data-stu-id="e15df-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="e15df-109">Klikk velg et **felt ved** siden av Gjør **følgende-feltet.**</span><span class="sxs-lookup"><span data-stu-id="e15df-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="e15df-110">Velg **Krypter i** rullegardinmenyen for RMS-mal, og klikk deretter **OK.**</span><span class="sxs-lookup"><span data-stu-id="e15df-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="e15df-111">(Hvis du ikke ser dette alternativet, betyr det at planen ikke inkluderer automatisk kryptering.</span><span class="sxs-lookup"><span data-stu-id="e15df-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="e15df-112">Men du kan legge den til!)</span><span class="sxs-lookup"><span data-stu-id="e15df-112">But you can add it!)</span></span>
9. <span data-ttu-id="e15df-113">Velg et valgfritt valg (fra en liste over valgfrie valg som du kan gjøre på dette tidspunktet, og mange av dem kan etterlates med standardinnstillingen for enkelhets skyld).</span><span class="sxs-lookup"><span data-stu-id="e15df-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="e15df-114">Klikk på **Lagre**.</span><span class="sxs-lookup"><span data-stu-id="e15df-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e15df-115">Du kan alltids komme tilbake og redigere denne regelen senere.</span><span class="sxs-lookup"><span data-stu-id="e15df-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="e15df-116">Hvis du vil ha mer informasjon om hvordan du oppretter regler for kryptering, kan du se Definere regler for e-postflyt [for å kryptere e-postmeldinger i Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="e15df-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>