---
title: 1491-søk-ikke-returnerende forventede-resultater
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709236"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="2a2e8-102">Innholdssøk returnerer ikke forventede resultater</span><span class="sxs-lookup"><span data-stu-id="2a2e8-102">Content Search not returning expected results</span></span>

<span data-ttu-id="2a2e8-103">Når du kjører innholdssøk fra Microsoft 365-sikkerhets& compliance Center, kan du få uventede søkeresultater.</span><span class="sxs-lookup"><span data-stu-id="2a2e8-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="2a2e8-104">Vurder følgende ting som kan påvirke søkeresultatene dine:</span><span class="sxs-lookup"><span data-stu-id="2a2e8-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="2a2e8-105">**Innholdsplasseringer og søkebetingelser**: Kontroller at du har valgt de riktige innholdsplasseringene og søkebetingelsene.</span><span class="sxs-lookup"><span data-stu-id="2a2e8-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="2a2e8-106">Hvis du kjørte et stort søk (med mange steder), kan du vurdere å dele det opp i flere søk.</span><span class="sxs-lookup"><span data-stu-id="2a2e8-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="2a2e8-107">**Delvis indekserte elementer:** [Delvis indekserte elementer](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) fra postbokser er inkludert i de estimerte søkeresultatene.</span><span class="sxs-lookup"><span data-stu-id="2a2e8-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="2a2e8-108">Delvis indekserte elementer fra områder i SharePoint og OneDrive er imidlertid ikke inkludert i søkeestimatet.</span><span class="sxs-lookup"><span data-stu-id="2a2e8-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="2a2e8-109">**Søkefeil:** Når du søker i et stort antall postbokser (over 100 000 postbokser), kan du få søkefeil, med feilkoder som CS008-009 og CS012-002).</span><span class="sxs-lookup"><span data-stu-id="2a2e8-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="2a2e8-110">I dette tilfellet kan du prøve søket bare for de mislykkede innholdsplasseringene.</span><span class="sxs-lookup"><span data-stu-id="2a2e8-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="2a2e8-111">Se [denne artikkelen](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="2a2e8-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
