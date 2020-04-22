---
title: S/MIME i Outlook på nettet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764881"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="ff2bb-102">Krypter e-postmeldinger i Outlook</span><span class="sxs-lookup"><span data-stu-id="ff2bb-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="ff2bb-103">Microsoft 365 Message Encryption er bygget på Microsoft Azure Rights Management (Azure RMS), som er en del av Azure Information Protection.</span><span class="sxs-lookup"><span data-stu-id="ff2bb-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="ff2bb-104">Hvis abonnementet inkluderer Azure Rights Management eller Azure Information Protection, **trenger du ikke å gjøre noen handlinger for å aktivere eller aktivere** Rights Management-tjenesten manuelt.</span><span class="sxs-lookup"><span data-stu-id="ff2bb-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="ff2bb-105">Basert på tilbakemeldinger fra kunder, vil vi ikke lenger aktivere Exchange-regler for e-postflyt for automatisk å kryptere utgående e-post som inneholder visse typer sensitiv informasjon i leieren som standard.</span><span class="sxs-lookup"><span data-stu-id="ff2bb-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="ff2bb-106">I stedet gir vi detaljerte instruksjoner om hvordan dere kan gjøre det selv.</span><span class="sxs-lookup"><span data-stu-id="ff2bb-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="ff2bb-107">Hvis du vil ha mer informasjon om hvordan du oppretter en transportregel for å kryptere sensitiv informasjon, kan du se [denne artikkelen](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="ff2bb-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="ff2bb-108">Hvis du bruker Outlook på weben (tidligere **OWA**): Når du skriver en e-postmelding, klikker du bare **Beskytt** i OWA.</span><span class="sxs-lookup"><span data-stu-id="ff2bb-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="ff2bb-109">Dette vil gjelde "Ikke videresend" tillatelse.</span><span class="sxs-lookup"><span data-stu-id="ff2bb-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="ff2bb-110">Klikk **Endre tillatelse,** og velg **Krypter** for å bare kryptere meldingen.</span><span class="sxs-lookup"><span data-stu-id="ff2bb-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="ff2bb-111">Hvis du bruker **Outlook-klient:** Hvis du vil sende en kryptert melding fra Outlook 2013 eller 2016 eller Outlook 2016 for Mac, velger du > **Alternativer-tillatelser**, og deretter velger du beskyttelsesalternativet du trenger. **Options**</span><span class="sxs-lookup"><span data-stu-id="ff2bb-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="ff2bb-112">Hvis du vil **kryptere all e-post** som sendes til bestemte mottakere eller eksterne partnerorganisasjoner, må du opprette en regel for transport av e-postflyt i administrasjonssenteret for Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff2bb-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="ff2bb-113">Detaljerte instruksjoner er gitt i [denne støtteartikkelen](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="ff2bb-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

