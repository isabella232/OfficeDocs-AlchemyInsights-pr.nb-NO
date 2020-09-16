---
title: 1491 – søk – ikke returnert – forventet resultat
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740483"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="22aba-102">Innholds søk returnerer ikke forventede resultater</span><span class="sxs-lookup"><span data-stu-id="22aba-102">Content Search not returning expected results</span></span>

<span data-ttu-id="22aba-103">Når du kjører innholds søk fra sikkerhets & Samsvars senteret i Microsoft 365, kan det hende du får uventede søke resultater.</span><span class="sxs-lookup"><span data-stu-id="22aba-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="22aba-104">Vurder følgende ting som kan påvirke søke resultatene:</span><span class="sxs-lookup"><span data-stu-id="22aba-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="22aba-105">**Innholds plasseringer og søke betingelser**: Kontroller at du har valgt riktige innholds plasseringer og søke vilkårene.</span><span class="sxs-lookup"><span data-stu-id="22aba-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="22aba-106">Hvis du kjørte et stort søk (med mange plasseringer), bør du vurdere å dele det inn i flere søk.</span><span class="sxs-lookup"><span data-stu-id="22aba-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="22aba-107">**Delvis indekserte elementer**:  [delvis indekserte elementer](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) fra post bokser er inkludert i de beregnede søke resultatene.</span><span class="sxs-lookup"><span data-stu-id="22aba-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="22aba-108">Delvis indekserte elementer fra nett steder i SharePoint og OneDrive er imidlertid ikke inkludert i søke estimatet.</span><span class="sxs-lookup"><span data-stu-id="22aba-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="22aba-109">**Søke feil**: Når du søker etter et stort antall post bokser (over 100 000 post bokser), kan du få søke feil, med feil koder som CS008-009 og CS012-002).</span><span class="sxs-lookup"><span data-stu-id="22aba-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="22aba-110">I dette tilfellet må du prøve søket på nytt bare for de mislykkede innholds plasseringene.</span><span class="sxs-lookup"><span data-stu-id="22aba-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="22aba-111">Se  [denne artikkelen](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) hvis du vil ha mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="22aba-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
