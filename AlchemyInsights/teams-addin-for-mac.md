---
title: Teams-tillegget for Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629743"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="c5b6e-102">Teams-tillegget for Mac</span><span class="sxs-lookup"><span data-stu-id="c5b6e-102">Teams add-in for Mac</span></span>

<span data-ttu-id="c5b6e-103">Følg denne Fremgangs måten for å feilsøke et manglende Teams-tillegg for Mac-brukere av operativ systemet:</span><span class="sxs-lookup"><span data-stu-id="c5b6e-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="c5b6e-104">**Trinn 1:** Hvis du har hybrid Exchange lokalt (2016 CU3 eller senere kreves), bruker du Test-HMA.ps1-verktøyet til å bekrefte at hybrid moderne godkjenning er riktig konfigurert.</span><span class="sxs-lookup"><span data-stu-id="c5b6e-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="c5b6e-105">Hvis du vil ha mer informasjon, kan du se [validere hybrid moderne godkjennings konfigurasjon for Outlook for IOS og Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="c5b6e-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="c5b6e-106">**Obs!** Bruk UPN-adresse formatet (for eksempel [username@contoso.com](mailto:username@contoso.com)), ikke Domain\Username.</span><span class="sxs-lookup"><span data-stu-id="c5b6e-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="c5b6e-107">Gjør dette selv for brukere med Exchange Online-postbokser.</span><span class="sxs-lookup"><span data-stu-id="c5b6e-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="c5b6e-108">**Trinn 2:** Få brukeren til å gå til **verktøy**  >  **kontoer**... i Outlook for Mac, og Finn og velg kontoen.</span><span class="sxs-lookup"><span data-stu-id="c5b6e-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="c5b6e-109">Bekreft at bruker navnet som er oppført, er i UPN-format (for eksempel [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="c5b6e-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="c5b6e-110">**Trinn 3:** Bekreft at brukeren er en lisensiert Microsoft Teams-bruker.</span><span class="sxs-lookup"><span data-stu-id="c5b6e-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="c5b6e-111">Brukeren må bruke Office 365 for Mac-abonnementet, produkt versjon 16,24 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="c5b6e-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>