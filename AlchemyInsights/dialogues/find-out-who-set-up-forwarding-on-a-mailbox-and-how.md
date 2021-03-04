---
title: Finne ut hvem som konfigurerte videresending for en postboks, og hvordan
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429989"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="0ced1-102">Finne ut hvem som konfigurerte videresending for en postboks, og hvordan</span><span class="sxs-lookup"><span data-stu-id="0ced1-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="0ced1-103">Hvis ekstern videresending ble satt på en postboks, overvåkes aktiviteten som en del Set-Mailbox cmdlet.</span><span class="sxs-lookup"><span data-stu-id="0ced1-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="0ced1-104">Slik finner du aktiviteten i overvåkingsloggen:</span><span class="sxs-lookup"><span data-stu-id="0ced1-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="0ced1-105">Gå til [sikkerhetssenteret for Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="0ced1-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="0ced1-106">Velg **søk i** >  **overvåkingsloggen** for søk.</span><span class="sxs-lookup"><span data-stu-id="0ced1-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="0ced1-107">Hvis du ser en melding om at du må aktivere overvåking, går du videre og slår den på nå.</span><span class="sxs-lookup"><span data-stu-id="0ced1-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="0ced1-108">Hvis denne funksjonen ikke er aktivert, kan ikke søkeresultatene hente data fra tidligere datoer.</span><span class="sxs-lookup"><span data-stu-id="0ced1-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="0ced1-109">Kontroller at **Aktiviteter-feltet** er satt til **Vis resultater for alle aktiviteter** (standard).</span><span class="sxs-lookup"><span data-stu-id="0ced1-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="0ced1-110">Angi datoområdet.</span><span class="sxs-lookup"><span data-stu-id="0ced1-110">Specify the date range.</span></span> <span data-ttu-id="0ced1-111">Du trenger ikke å angi et brukernavn.</span><span class="sxs-lookup"><span data-stu-id="0ced1-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="0ced1-112">Velg **Søk.**</span><span class="sxs-lookup"><span data-stu-id="0ced1-112">Select **Search**.</span></span> <span data-ttu-id="0ced1-113">Aktivitetene vises under **Resultater.**</span><span class="sxs-lookup"><span data-stu-id="0ced1-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="0ced1-114">Velg **Filterresultater,** og angi **deretter Set-mailbox** i **Aktivitetsfilter-feltet.**</span><span class="sxs-lookup"><span data-stu-id="0ced1-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="0ced1-115">Dette returnerer alle **Set-Mailbox-aktiviteter.**</span><span class="sxs-lookup"><span data-stu-id="0ced1-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="0ced1-116">Hvis du vil vise detaljene, velger du en aktivitet og velger **deretter Mer informasjon.**</span><span class="sxs-lookup"><span data-stu-id="0ced1-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="0ced1-117">Under **Parametere** kan du se e-postadressen for videresending som ble angitt for postboksen.</span><span class="sxs-lookup"><span data-stu-id="0ced1-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="0ced1-118">**Bruker-ID-en** representerer brukeren som konfigurerte ekstern videresending for postboksen.</span><span class="sxs-lookup"><span data-stu-id="0ced1-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="0ced1-119">Hvis du vil ha mer informasjon, kan du se Søke i overvåkingsloggen for [Office 365 for å feilsøke vanlige scenarioer.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="0ced1-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>