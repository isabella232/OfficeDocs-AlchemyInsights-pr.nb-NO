---
title: 1491-søk-ikke-returnerende-forventede resultater
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
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510581"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="3c042-102">Innholdssøk returnerer ikke forventede resultater</span><span class="sxs-lookup"><span data-stu-id="3c042-102">Content Search not returning expected results</span></span>

<span data-ttu-id="3c042-103">Når du kjører innholdssøk fra Sikkerhets- & Samsvarssenter for Microsoft 365, kan du få uventede søkeresultater.</span><span class="sxs-lookup"><span data-stu-id="3c042-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="3c042-104">Vurder følgende ting som kan påvirke søkeresultatene dine:</span><span class="sxs-lookup"><span data-stu-id="3c042-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="3c042-105">**Innholdsplasseringer og søkebetingelser**: Kontroller at du har valgt de riktige innholdsplasseringene og søkevilkårene.</span><span class="sxs-lookup"><span data-stu-id="3c042-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="3c042-106">Hvis du kjørte et stort søk (med mange steder), bør du vurdere å dele det opp i flere søk.</span><span class="sxs-lookup"><span data-stu-id="3c042-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="3c042-107">**Delvis indekserte elementer**: [Delvis indekserte elementer](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) fra postbokser er inkludert i de estimerte søkeresultatene.</span><span class="sxs-lookup"><span data-stu-id="3c042-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="3c042-108">Delvis indekserte elementer fra områder i SharePoint og OneDrive er imidlertid ikke inkludert i søkeestimatet.</span><span class="sxs-lookup"><span data-stu-id="3c042-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="3c042-109">**Søksfeil**: Når du søker i et stort antall postbokser (over 100 000 postbokser), kan du få søkefeil, med feilkoder som CS008-009 og CS012-002).</span><span class="sxs-lookup"><span data-stu-id="3c042-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="3c042-110">I dette tilfellet prøver du søket bare etter de mislykkede innholdsplasseringene.</span><span class="sxs-lookup"><span data-stu-id="3c042-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="3c042-111">Se [denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="3c042-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
