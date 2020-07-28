---
title: Flere objekter har samme e-postadresse som identitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439189"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a><span data-ttu-id="6f2d7-102">Flere objekter har samme e-postadresse som identitet</span><span class="sxs-lookup"><span data-stu-id="6f2d7-102">Multiple objects have the same email address as identity</span></span>

<span data-ttu-id="6f2d7-103">**Flere objekter**</span><span class="sxs-lookup"><span data-stu-id="6f2d7-103">**Multiple objects**</span></span>

<span data-ttu-id="6f2d7-104">En av de vanligste årsakene til denne feilen er ikke å kunne rute en Outlook Web Access-forespørsel riktig i en tilstedeværelse av flere objekter som har samme e-postadresse som identitet.</span><span class="sxs-lookup"><span data-stu-id="6f2d7-104">One of the common reasons of this error is not being able to route an Outlook Web Access request properly in a presence of multiple objects having the same email address as identity.</span></span> <span data-ttu-id="6f2d7-105">Hvis du vil finne disse objektene, kjører du følgende kommandoer:</span><span class="sxs-lookup"><span data-stu-id="6f2d7-105">To find these objects, run the following commands:</span></span>

<span data-ttu-id="6f2d7-106">· Få-mottaker<email address></span><span class="sxs-lookup"><span data-stu-id="6f2d7-106">· Get-Recipient <email address></span></span>

<span data-ttu-id="6f2d7-107">· Få-bruker<email address></span><span class="sxs-lookup"><span data-stu-id="6f2d7-107">· Get-User <email address></span></span>

<span data-ttu-id="6f2d7-108">· Få bruker <email address> -SoftDeletedUser</span><span class="sxs-lookup"><span data-stu-id="6f2d7-108">· Get-User <email address> -SoftDeletedUser</span></span>

<span data-ttu-id="6f2d7-109">· Få kontakt<email address></span><span class="sxs-lookup"><span data-stu-id="6f2d7-109">· Get-Contact <email address></span></span>

<span data-ttu-id="6f2d7-110">· Get-Postboks <email address> - PublicFolder</span><span class="sxs-lookup"><span data-stu-id="6f2d7-110">· Get-Mailbox <email address> -PublicFolder</span></span>

<span data-ttu-id="6f2d7-111">· Get-Postboks <email address> -IncludeSoftDeletedMailbox</span><span class="sxs-lookup"><span data-stu-id="6f2d7-111">· Get-Mailbox <email address> -IncludeSoftDeletedMailbox</span></span>

<span data-ttu-id="6f2d7-112">· Get-Postboks <email address> -InaktivMailboxBare</span><span class="sxs-lookup"><span data-stu-id="6f2d7-112">· Get-Mailbox <email address> -InactiveMailboxOnly</span></span>

<span data-ttu-id="6f2d7-113">Hvis du vil løse problemet, kan du fjerne flere objekter med samme e-postidentitet og kontrollere at det er ett enkelt objekt med den bestemte e-postidentiteten, og at mottakertypen er UserMailbox.</span><span class="sxs-lookup"><span data-stu-id="6f2d7-113">To resolve the issue, remove multiple objects with the same email identity and make sure that there is a single object with the specific email identity and that its recipient type is UserMailbox.</span></span>

<span data-ttu-id="6f2d7-114">**Samme adresse brukes for forretnings- og forbrukerpostbokser**</span><span class="sxs-lookup"><span data-stu-id="6f2d7-114">**Same address is used for business and consumer mailboxes**</span></span>

<span data-ttu-id="6f2d7-115">En annen årsak er når den samme adressen brukes for forretnings- og forbrukerpostbokser.</span><span class="sxs-lookup"><span data-stu-id="6f2d7-115">Another cause is when the same address is used for business and consumer mailboxes.</span></span> <span data-ttu-id="6f2d7-116">I dette tilfellet må brukeren endre sitt primære forbrukeralias til Cafe støtter dette scenariet.</span><span class="sxs-lookup"><span data-stu-id="6f2d7-116">In this case, the user must change their primary consumer alias until Cafe supports this scenario.</span></span> <span data-ttu-id="6f2d7-117">Dette er en permanent feil som ikke går bort uten inngripen.</span><span class="sxs-lookup"><span data-stu-id="6f2d7-117">This is a permanent error that does not go away without intervention.</span></span>

<span data-ttu-id="6f2d7-118">Hvis du vil ha mer informasjon, kan du se [Endre e-postadressen eller telefonnummeret for Microsoft-kontoen](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span><span class="sxs-lookup"><span data-stu-id="6f2d7-118">For details, see [Change the email address or phone number for your Microsoft account](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).</span></span>