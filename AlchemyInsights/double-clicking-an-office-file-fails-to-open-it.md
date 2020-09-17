---
title: Når du dobbelt klikker en Office-fil, åpnes den ikke
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812088"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="4b0f5-102">Når du dobbelt klikker en Office-fil, åpnes den ikke</span><span class="sxs-lookup"><span data-stu-id="4b0f5-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="4b0f5-103">Når du har dobbelt klikket en Office-fil, kan du se programmet åpent, men selve filen åpnes ikke.</span><span class="sxs-lookup"><span data-stu-id="4b0f5-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="4b0f5-104">Eller du kan få feil meldingen «det oppstod et problem ved sending av kommandoen til programmet.»</span><span class="sxs-lookup"><span data-stu-id="4b0f5-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="4b0f5-105">Det er mange årsaker til dette, men de to vanligste løsningene er:</span><span class="sxs-lookup"><span data-stu-id="4b0f5-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="4b0f5-106">Kontroller at DDE-alternativet ikke er avmerket i Excel.</span><span class="sxs-lookup"><span data-stu-id="4b0f5-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="4b0f5-107">Du kan finne alternativet ved å opprette en ny arbeids bok og deretter velge **Alternativer for fil > > avansert**.</span><span class="sxs-lookup"><span data-stu-id="4b0f5-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="4b0f5-108">Fjern merket for **Ignorer andre programmer som bruker dynamisk data utveksling (DDE)**, i **Generelt** -delen.</span><span class="sxs-lookup"><span data-stu-id="4b0f5-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="4b0f5-109">Kjør en tilkoblet reparasjon for å gjenopprette standard innstillingene.</span><span class="sxs-lookup"><span data-stu-id="4b0f5-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="4b0f5-110">Klikk Start knappen i Windows, og søk etter kontroll panel.</span><span class="sxs-lookup"><span data-stu-id="4b0f5-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="4b0f5-111">Åpne **kontroll panel**, og gå til **programmer > programmer og funksjoner**.</span><span class="sxs-lookup"><span data-stu-id="4b0f5-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="4b0f5-112">Høyre klikk deretter **Microsoft Office [versjon]** , og velg **endre > elektronisk reparasjon**.</span><span class="sxs-lookup"><span data-stu-id="4b0f5-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="4b0f5-113">Hvis ingen av disse løsningene fungerer, kan du finne en mer komplett liste over løsninger i kunde støtte artikkelen ved [å dobbeltklikke en Office-fil som ikke åpner den](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="4b0f5-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
