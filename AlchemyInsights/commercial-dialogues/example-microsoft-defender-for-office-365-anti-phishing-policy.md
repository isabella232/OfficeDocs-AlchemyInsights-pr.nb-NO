---
title: Eksempel på Microsoft Defender for office 365-policy mot phishing
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
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750791"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="bac0b-102">Eksempel på Microsoft Defender for office 365-policy mot phishing</span><span class="sxs-lookup"><span data-stu-id="bac0b-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="bac0b-103">Disse innstillingene aktiverer en policy kalt *Domene og ADMINISTRERENDE DIREKTØR.*</span><span class="sxs-lookup"><span data-stu-id="bac0b-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="bac0b-104">Denne policyen gir både bruker- og domenebeskyttelse mot representasjon og bruker deretter policyen på all e-post som mottas av brukere i domenet.</span><span class="sxs-lookup"><span data-stu-id="bac0b-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="bac0b-105">Først legger du til følgende informasjon for å opprette policyen:</span><span class="sxs-lookup"><span data-stu-id="bac0b-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="bac0b-106">**Navn:** Beskrivelse av domene **og administrerende direktør**: Sikrer at administrerende direktør og domenet ikke representeres.</span><span class="sxs-lookup"><span data-stu-id="bac0b-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="bac0b-107">**Brukes på:** Velg **Mottakerdomenet er**.</span><span class="sxs-lookup"><span data-stu-id="bac0b-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="bac0b-108">Velg **Velg under Hvilken som** helst av disse , og velg deretter et domene. </span><span class="sxs-lookup"><span data-stu-id="bac0b-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="bac0b-109">Velg **+ Legg til**.</span><span class="sxs-lookup"><span data-stu-id="bac0b-109">Select **+ Add**.</span></span> <span data-ttu-id="bac0b-110">Merk av for navnet på domenet i listen (for eksempel contoso.com *),* og velg deretter **Legg til**.</span><span class="sxs-lookup"><span data-stu-id="bac0b-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="bac0b-111">Velg **Ferdig**.</span><span class="sxs-lookup"><span data-stu-id="bac0b-111">Select **Done**.</span></span>
- <span data-ttu-id="bac0b-112">Når policyen er opprettet, kan du finjustere policyen ved hjelp av følgende alternativer:</span><span class="sxs-lookup"><span data-stu-id="bac0b-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="bac0b-113">**Legg til brukere for å beskytte:** I dette eksemplet kan du legge til konsernsjefens e-postadresse, som et minimum.</span><span class="sxs-lookup"><span data-stu-id="bac0b-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="bac0b-114">**Legg til domener for å beskytte**: Legg til organisasjonsdomenet som inkluderer kontoret til administrerende direktør.</span><span class="sxs-lookup"><span data-stu-id="bac0b-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="bac0b-115">**Velg handlinger:** **Hvis** e-post sendes av en representasjonsbruker , velger du Omadresser melding til en annen e-postadresse **,** og deretter skriver du inn e-postadressen til sikkerhetsadministratoren (for eksempel *securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="bac0b-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="bac0b-116">For **Hvis e-post sendes av et etterlignet domene**, velger du **Karantene meldingen**.</span><span class="sxs-lookup"><span data-stu-id="bac0b-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="bac0b-117">**Postboksintelligens:** Dette alternativet velges som standard når du oppretter en ny phishing-policy.</span><span class="sxs-lookup"><span data-stu-id="bac0b-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="bac0b-118">La denne innstillingen **være På** for å få best resultat.</span><span class="sxs-lookup"><span data-stu-id="bac0b-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="bac0b-119">**Legg til klarerte avsendere og domener:** I dette eksemplet må du ikke definere noen overstyringer.</span><span class="sxs-lookup"><span data-stu-id="bac0b-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="bac0b-120">Når du har gått gjennom innstillingene, velger du **Opprett denne policyen** eller **Lagre** etter behov.</span><span class="sxs-lookup"><span data-stu-id="bac0b-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="bac0b-121">Hvis du vil ha mer informasjon, kan du se [Phishing-policyer i Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="bac0b-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
