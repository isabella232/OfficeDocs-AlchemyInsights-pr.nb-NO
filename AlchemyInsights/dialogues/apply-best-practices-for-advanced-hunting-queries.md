---
title: Bruk anbefalte fremgangsmåter for avanserte søk
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
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696089"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="d092a-102">Bruk anbefalte fremgangsmåter for avanserte søk</span><span class="sxs-lookup"><span data-stu-id="d092a-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="d092a-103">Bruk disse anbefalte fremgangsmåtene for å få resultater raskere og unngå tidsavbrudd når du kjører komplekse spørringer:</span><span class="sxs-lookup"><span data-stu-id="d092a-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="d092a-104">Når du prøver nye spørringer, bør du alltid bruke en grense for å unngå å få svært store resultatsett.</span><span class="sxs-lookup"><span data-stu-id="d092a-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="d092a-105">Bruk også denne til å gjøre en innledende vurdering av størrelsen `count` på resultatsettet.</span><span class="sxs-lookup"><span data-stu-id="d092a-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="d092a-106">Bruk tidsfiltre først.</span><span class="sxs-lookup"><span data-stu-id="d092a-106">Use time filters first.</span></span> <span data-ttu-id="d092a-107">Ideelt sett bør du begrense spørringene til sju dager.</span><span class="sxs-lookup"><span data-stu-id="d092a-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="d092a-108">I begynnelsen av en spørring, rett etter tidsfilteret, legger du til filtrene som forventes å fjerne mesteparten av dataene.</span><span class="sxs-lookup"><span data-stu-id="d092a-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="d092a-109">Når du leter etter fullstendige tokener, bruker du `has` operatoren i stedet for `contains` .</span><span class="sxs-lookup"><span data-stu-id="d092a-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="d092a-110">Kjør et søk på en bestemt kolonne i stedet for på tvers av alle kolonner.</span><span class="sxs-lookup"><span data-stu-id="d092a-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="d092a-111">Når du føyer sammen tabeller, må du først angi tabellen med færre rader.</span><span class="sxs-lookup"><span data-stu-id="d092a-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="d092a-112">`project` bare de nødvendige kolonnene fra tabellene du har sammenføyd.</span><span class="sxs-lookup"><span data-stu-id="d092a-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="d092a-113">Hvis du vil ha mer informasjon, kan du [se anbefalte fremgangsmåter for avansert søk for søk.](https://go.microsoft.com/fwlink/?linkid=2144812)</span><span class="sxs-lookup"><span data-stu-id="d092a-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
