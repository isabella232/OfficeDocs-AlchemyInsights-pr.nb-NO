---
title: Store SharePoint-lister
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488526"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="66d01-102">Arbeide med store lister og biblioteker i SharePoint</span><span class="sxs-lookup"><span data-stu-id="66d01-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="66d01-103">SharePoint-lister og-biblioteker kan inneholde opptil 30 000 000 elementer, men når de har mer enn 5 000 elementer, kan det hende du ser en terskelverdi for listevisning når du prøver å arbeide med dem.</span><span class="sxs-lookup"><span data-stu-id="66d01-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="66d01-104">Denne terskelen er på plass for å opprettholde ytelsen til tjenesten.</span><span class="sxs-lookup"><span data-stu-id="66d01-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="66d01-105">Den kan ikke endres.</span><span class="sxs-lookup"><span data-stu-id="66d01-105">It can't be changed.</span></span> <span data-ttu-id="66d01-106">For å unngå å treffe denne terskelen:</span><span class="sxs-lookup"><span data-stu-id="66d01-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="66d01-107">**Bruk moderne**</span><span class="sxs-lookup"><span data-stu-id="66d01-107">**Use modern**</span></span>

<span data-ttu-id="66d01-108">Visninger som viser mange elementer fungerer best i den moderne opplevelsen.</span><span class="sxs-lookup"><span data-stu-id="66d01-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="66d01-109">[Bruk den moderne opplevelsen](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) for å unngå feil du kan se i den klassiske opplevelsen.</span><span class="sxs-lookup"><span data-stu-id="66d01-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="66d01-110">**Legge til indekser**</span><span class="sxs-lookup"><span data-stu-id="66d01-110">**Add indexes**</span></span>

<span data-ttu-id="66d01-111">Når du filtrerer eller sorterer etter en kolonne som ikke har en indeks, kan det hende du ser en feilmelding.</span><span class="sxs-lookup"><span data-stu-id="66d01-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="66d01-112">[Legg til en indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuelt fra **listeinnstillinger** i innstillingsmenyen, og deretter **indekserte kolonner**.</span><span class="sxs-lookup"><span data-stu-id="66d01-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="66d01-113">**Redigere listevisningen**</span><span class="sxs-lookup"><span data-stu-id="66d01-113">**Edit the list view**</span></span>

<span data-ttu-id="66d01-114">Hvis det oppstår en feil når du arbeider med en stor liste, [redigerer du listevisningen](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="66d01-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="66d01-115">Følgende fire endringer vil fjerne terskel feil for listevisning.</span><span class="sxs-lookup"><span data-stu-id="66d01-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="66d01-116">Gjør alle fire endringer for å fjerne alle feil.</span><span class="sxs-lookup"><span data-stu-id="66d01-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="66d01-117">Hvis du fremdeles får feilmeldinger, kontrollerer du [behandle store lister og biblioteker](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="66d01-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="66d01-118">Velg **ingen** fra både **første sortering etter kolonnen** , og **Sorter deretter etter kolonnen**.</span><span class="sxs-lookup"><span data-stu-id="66d01-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="66d01-119">Velg **ingen** fra både **første gruppe etter kolonnen** og **grupper deretter etter kolonnen**.</span><span class="sxs-lookup"><span data-stu-id="66d01-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="66d01-120">Velg **ingen** for alle kolonnene i **Totaler** -delen.</span><span class="sxs-lookup"><span data-stu-id="66d01-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="66d01-121">Opphev markeringen av alle unntatt én kolonne for visning fra **kolonner** -delen.</span><span class="sxs-lookup"><span data-stu-id="66d01-121">Deselect all but one column for display from the **Columns** section.</span></span>

