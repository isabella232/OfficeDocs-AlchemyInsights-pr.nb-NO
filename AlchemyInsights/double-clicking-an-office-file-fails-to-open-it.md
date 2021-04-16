---
title: Når du dobbeltklikker på en Office-fil, åpnes den ikke
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814814"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="9ba75-102">Når du dobbeltklikker på en Office-fil, åpnes den ikke</span><span class="sxs-lookup"><span data-stu-id="9ba75-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="9ba75-103">Når du har dobbeltklikket en Office-fil, kan det hende du ser at programmet er åpent, men selve filen åpnes ikke.</span><span class="sxs-lookup"><span data-stu-id="9ba75-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="9ba75-104">Eller du kan få feilmeldingen: «Det oppstod et problem under sending av kommandoen til programmet.»</span><span class="sxs-lookup"><span data-stu-id="9ba75-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="9ba75-105">Det finnes mange årsaker til dette, men de to vanligste løsningene er:</span><span class="sxs-lookup"><span data-stu-id="9ba75-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="9ba75-106">Kontroller at det ikke er merket av for DDE i Excel.</span><span class="sxs-lookup"><span data-stu-id="9ba75-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="9ba75-107">Du finner alternativet ved å opprette en ny arbeidsbok og deretter velge Fil > **Alternativer > Avansert**.</span><span class="sxs-lookup"><span data-stu-id="9ba75-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="9ba75-108">Fjern merket **for** Ignorer andre programmer som bruker **Dynamisk datautveksling (DDE)** under Generelt.</span><span class="sxs-lookup"><span data-stu-id="9ba75-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="9ba75-109">Kjør en tilkoblet reparasjon for å gjenopprette standardinnstillingene.</span><span class="sxs-lookup"><span data-stu-id="9ba75-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="9ba75-110">Klikk Start-knappen i Windows, og søk etter «Kontrollpanel».</span><span class="sxs-lookup"><span data-stu-id="9ba75-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="9ba75-111">Åpne Kontrollpanel **, og** gå til Programmer > Programmer **og funksjoner**.</span><span class="sxs-lookup"><span data-stu-id="9ba75-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="9ba75-112">Høyreklikk deretter **Microsoft Office [versjon]** og velg Endre > **tilkoblet reparasjon**.</span><span class="sxs-lookup"><span data-stu-id="9ba75-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="9ba75-113">Hvis ingen av disse løsningene fungerer, finner du en mer fullstendig liste over løsninger i støtteartikkelen. Dobbeltklikking av en [Office-fil](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)kan ikke åpne den .</span><span class="sxs-lookup"><span data-stu-id="9ba75-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
