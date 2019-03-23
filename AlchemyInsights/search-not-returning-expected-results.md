---
title: 1491-Search-not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776090"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="a8b30-102">Innhold Søk returnerer ikke forventet resultat</span><span class="sxs-lookup"><span data-stu-id="a8b30-102">Content Search not returning expected results</span></span>

<span data-ttu-id="a8b30-103">Når du kjører innhold søk fra Office 365-sikkerhet & Center-kompatibilitet, kan du få uventede resultater.</span><span class="sxs-lookup"><span data-stu-id="a8b30-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="a8b30-104">Vurder følgende ting som kan påvirke søkeresultatene:</span><span class="sxs-lookup"><span data-stu-id="a8b30-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="a8b30-105">**Plassering av innhold og søkebetingelser**: Kontroller at du har valgt riktig innholdsplasseringer og søkevilkårene.</span><span class="sxs-lookup"><span data-stu-id="a8b30-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="a8b30-106">Hvis du kjørte en stor Søk (med mange steder), kan du vurdere å dele den opp i flere søk.</span><span class="sxs-lookup"><span data-stu-id="a8b30-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="a8b30-107">**Delvis indekserte elementer**: [delvis indekserte elementer](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) fra postbokser inkluderes i beregnet søkeresultatene.</span><span class="sxs-lookup"><span data-stu-id="a8b30-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="a8b30-108">Imidlertid er delvis indekserte elementer fra områder i SharePoint og OneDrive ikke er inkludert i estimatet søk.</span><span class="sxs-lookup"><span data-stu-id="a8b30-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="a8b30-109">**Søk-feil**: Når du søker etter et stort antall postbokser (over 100 000 postbokser), kan du få feilmeldinger når søk, med feilkoder som CS008-009 og CS012-002).</span><span class="sxs-lookup"><span data-stu-id="a8b30-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="a8b30-110">I dette tilfellet, prøv Søk bare etter de mislykkede innholdsplasseringer.</span><span class="sxs-lookup"><span data-stu-id="a8b30-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="a8b30-111">Se [denne artikkelen](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="a8b30-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
