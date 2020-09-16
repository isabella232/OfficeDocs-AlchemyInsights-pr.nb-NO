---
title: Store lister i SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720142"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="9142d-102">Arbeide med store lister og biblioteker i SharePoint</span><span class="sxs-lookup"><span data-stu-id="9142d-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="9142d-103">SharePoint-lister og-biblioteker kan inneholde opptil 30 000 000 elementer, men når de har mer enn 5 000 elementer, kan det hende at det vises en terskel feil for liste visning når du prøver å arbeide med dem.</span><span class="sxs-lookup"><span data-stu-id="9142d-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="9142d-104">Denne terskelen er der for å opprettholde ytelsen til tjenesten.</span><span class="sxs-lookup"><span data-stu-id="9142d-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="9142d-105">Den kan ikke endres.</span><span class="sxs-lookup"><span data-stu-id="9142d-105">It can't be changed.</span></span> <span data-ttu-id="9142d-106">Slik unngår du å treffe denne terskelen:</span><span class="sxs-lookup"><span data-stu-id="9142d-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="9142d-107">**Bruke moderne**</span><span class="sxs-lookup"><span data-stu-id="9142d-107">**Use modern**</span></span>

<span data-ttu-id="9142d-108">Visninger som viser mange elementer fungerer best i den moderne opplevelsen.</span><span class="sxs-lookup"><span data-stu-id="9142d-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="9142d-109">[Bruk den moderne opplevelsen](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) til å unngå feil du kan se i den klassiske opplevelsen.</span><span class="sxs-lookup"><span data-stu-id="9142d-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="9142d-110">**Legge til indekser**</span><span class="sxs-lookup"><span data-stu-id="9142d-110">**Add indexes**</span></span>

<span data-ttu-id="9142d-111">Når du filtrerer eller sorterer etter en kolonne som ikke har en indeks, kan du se en feil melding.</span><span class="sxs-lookup"><span data-stu-id="9142d-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="9142d-112">[Legg til en indeks](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuelt fra **liste innstillinger** på Innstillinger-menyen, og deretter **indekserte kolonner**.</span><span class="sxs-lookup"><span data-stu-id="9142d-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="9142d-113">**Redigere liste visningen**</span><span class="sxs-lookup"><span data-stu-id="9142d-113">**Edit the list view**</span></span>

<span data-ttu-id="9142d-114">Hvis det oppstår en feil når du arbeider med en stor liste, kan [du redigere liste visningen](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="9142d-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="9142d-115">Følgende fire endringer vil fjerne terskel feil for liste visning.</span><span class="sxs-lookup"><span data-stu-id="9142d-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="9142d-116">Gjør alle de fire endringene for å fjerne alle feil.</span><span class="sxs-lookup"><span data-stu-id="9142d-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="9142d-117">Hvis du fortsatt får feil, må du kontrollere [behandle store lister og biblioteker](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="9142d-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="9142d-118">Velg **ingen** fra **den første Sorter etter kolonnen** , og **Sorter deretter etter kolonnen**.</span><span class="sxs-lookup"><span data-stu-id="9142d-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="9142d-119">Velg **ingen** fra **den første gruppen av kolonnen** , og **grupper deretter etter kolonnen**.</span><span class="sxs-lookup"><span data-stu-id="9142d-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="9142d-120">Velg **ingen** for alle Kol Onnene i **Totaler** -delen.</span><span class="sxs-lookup"><span data-stu-id="9142d-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="9142d-121">Fjern merket for alle unntatt én kolonne for visning fra **kolonner** -delen.</span><span class="sxs-lookup"><span data-stu-id="9142d-121">Deselect all but one column for display from the **Columns** section.</span></span>

