---
title: S/MIME i Outlook på nettet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772307"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="4eff6-102">Kryptere e-postmeldinger i Outlook</span><span class="sxs-lookup"><span data-stu-id="4eff6-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="4eff6-103">Microsoft 365-meldings kryptering er bygd på Microsoft Azure Rights Management (Azure RMS), som er en del av Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="4eff6-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="4eff6-104">Hvis abonnementet omfatter Azure Rights Management eller Azure Information Protection, **trenger du ikke utføre handlinger for å aktivere eller aktivere** Rights Management-tjenesten manuelt.</span><span class="sxs-lookup"><span data-stu-id="4eff6-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="4eff6-105">Avhengig av tilbake melding fra kunder, vil vi ikke lenger aktivere Exchange-regler for e-postflyter for automatisk kryptering av utgående e-post som inneholder bestemt type sensitiv informasjon i leieren din som standard.</span><span class="sxs-lookup"><span data-stu-id="4eff6-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="4eff6-106">I stedet gir vi detaljerte instruksjoner om hvordan du kan gjøre det selv.</span><span class="sxs-lookup"><span data-stu-id="4eff6-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="4eff6-107">Hvis du vil ha mer informasjon om hvordan du oppretter en transport regel for å kryptere sensitiv informasjon, kan du se [denne artikkelen](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="4eff6-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="4eff6-108">Hvis du bruker Outlook på nettet (tidligere **OWA**): Når du skriver en e-postmelding, klikker du bare **Beskytt** i OWA.</span><span class="sxs-lookup"><span data-stu-id="4eff6-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="4eff6-109">Dette vil bruke «ikke Videresend»-tillatelsen.</span><span class="sxs-lookup"><span data-stu-id="4eff6-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="4eff6-110">Klikk **endre tillatelse** , og velg **Krypter** for å bare kryptere meldingen.</span><span class="sxs-lookup"><span data-stu-id="4eff6-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="4eff6-111">Hvis du bruker **Outlook-klient**: Hvis du vil sende en kryptert melding fra Outlook 2013 eller 2016, eller Outlook 2016 for Mac, velger du **Alternativer**  >  -**tillatelser**, og deretter velger du beskyttelses alternativet du trenger.</span><span class="sxs-lookup"><span data-stu-id="4eff6-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="4eff6-112">Hvis du vil **kryptere alle e-postmeldinger** som er sendt til bestemte mottakere eller eksterne partner organisasjoner automatisk, må du opprette en e-postflyt transport regel i administrasjons senteret for Exchange.</span><span class="sxs-lookup"><span data-stu-id="4eff6-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="4eff6-113">Du finner detaljerte instruksjoner i [denne kunde støtte artikkelen](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="4eff6-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

