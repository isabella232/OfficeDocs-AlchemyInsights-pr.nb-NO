---
title: Teams for Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582079"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="96540-102">Teams for Mac</span><span class="sxs-lookup"><span data-stu-id="96540-102">Teams add-in for Mac</span></span>

<span data-ttu-id="96540-103">Følg disse trinnene for å feilsøke Teams for Mac-operativsystembrukere:</span><span class="sxs-lookup"><span data-stu-id="96540-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="96540-104">**Trinn 1:** Hvis du har hybrid Exchange lokalt (2016 CU3 eller nyere kreves), bruker du Test-HMA.ps1-verktøyet til å bekrefte at hybrid moderne godkjenning er riktig konfigurert.</span><span class="sxs-lookup"><span data-stu-id="96540-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="96540-105">Hvis du vil ha mer informasjon, kan du se Validere konfigurasjon av hybrid moderne [godkjenning for Outlook for iOS og Android.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="96540-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="96540-106">**Obs!** Bruk UPN-adresseformatet (for eksempel username@contoso.com [),](mailto:username@contoso.com)ikke domene\brukernavn.</span><span class="sxs-lookup"><span data-stu-id="96540-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="96540-107">Gjør dette selv for brukere med Exchange Online postbokser.</span><span class="sxs-lookup"><span data-stu-id="96540-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="96540-108">**Trinn 2:** Be brukeren gå til **Verktøykontoer**  >  ... i Outlook for Mac, og finn og velg kontoen.</span><span class="sxs-lookup"><span data-stu-id="96540-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="96540-109">Bekreft at brukernavnet som er oppført, er i UPN-format (for [eksempel username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="96540-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="96540-110">**Trinn 3:** Bekreft at brukeren er en lisensiert Microsoft Teams bruker.</span><span class="sxs-lookup"><span data-stu-id="96540-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="96540-111">Brukeren må bruke abonnementet Office 365 for Mac, produkt versjon 16.24 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="96540-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>