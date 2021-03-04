---
title: Finne IP-adressen i overvåkingsloggen
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429785"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="728d5-102">Finne IP-adressen i overvåkingsloggen</span><span class="sxs-lookup"><span data-stu-id="728d5-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="728d5-103">IP-adressen som tilsvarer en aktivitet utført av en bruker eller administrator, vises i overvåkingsloggene.</span><span class="sxs-lookup"><span data-stu-id="728d5-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="728d5-104">Klientinformasjonen logges også.</span><span class="sxs-lookup"><span data-stu-id="728d5-104">The client information is also logged.</span></span> <span data-ttu-id="728d5-105">Slik identifiserer du IP-adressen:</span><span class="sxs-lookup"><span data-stu-id="728d5-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="728d5-106">Gå til [sikkerhetssenteret for Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="728d5-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="728d5-107">Velg **søk i**  >  **[overvåkingsloggen](https://go.microsoft.com/fwlink/?linkid=2103759)** for søk.</span><span class="sxs-lookup"><span data-stu-id="728d5-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="728d5-108">Hvis du ser en melding om at du må aktivere overvåking, går du videre og slår den på nå.</span><span class="sxs-lookup"><span data-stu-id="728d5-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="728d5-109">Hvis denne funksjonen ikke er aktivert, kan ikke søkeresultatene hente data fra tidligere datoer.</span><span class="sxs-lookup"><span data-stu-id="728d5-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="728d5-110">Hvis du er interessert i en bestemt aktivitet, velger du den fra **Aktiviteter-listen.** Hvis ikke returneres alle aktiviteter for den valgte brukeren som standard.</span><span class="sxs-lookup"><span data-stu-id="728d5-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="728d5-111">Vær oppmerksom på at enkelte aktiviteter kanskje ikke er tilgjengelige for valg fra **Aktiviteter-menyen.** Disse overvåkingselementene returneres imidlertid hvis **Vis resultater for alle aktiviteter** er valgt (standardinnstilling).</span><span class="sxs-lookup"><span data-stu-id="728d5-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="728d5-112">Angi datoområdet, og velg **brukernavnet** for brukeren du vil undersøke, i Brukere-feltet.</span><span class="sxs-lookup"><span data-stu-id="728d5-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="728d5-113">Velg **Søk.**</span><span class="sxs-lookup"><span data-stu-id="728d5-113">Select **Search**.</span></span> <span data-ttu-id="728d5-114">Aktivitetene vises under **Resultater.**</span><span class="sxs-lookup"><span data-stu-id="728d5-114">The activities appear under **Results**.</span></span> <span data-ttu-id="728d5-115">Du kan se IP-adressen for hver aktivitet.</span><span class="sxs-lookup"><span data-stu-id="728d5-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="728d5-116">Hvis du vil vise detaljer, velger du en aktivitet og velger **deretter Mer informasjon.**</span><span class="sxs-lookup"><span data-stu-id="728d5-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="728d5-117">Hvis du vil ha mer informasjon, kan du se Søke i overvåkingsloggen for [Office 365 for å feilsøke vanlige scenarioer.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="728d5-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>