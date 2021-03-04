---
title: Les overvåkingsloggene for slettede hendelser
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429828"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="4d4d1-102">Les overvåkingsloggene for slettede hendelser</span><span class="sxs-lookup"><span data-stu-id="4d4d1-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="4d4d1-103">Slik gjør du det:</span><span class="sxs-lookup"><span data-stu-id="4d4d1-103">Here's how to do this:</span></span>

1. <span data-ttu-id="4d4d1-104">Gå til [sikkerhetssenteret for Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="4d4d1-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="4d4d1-105">Velg **søk i**  >  [**overvåkingsloggen**](https://go.microsoft.com/fwlink/?linkid=2103759)for søk.</span><span class="sxs-lookup"><span data-stu-id="4d4d1-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="4d4d1-106">Hvis du ser et varsel om at du må aktivere funksjonen, kan du bare slå den på nå.</span><span class="sxs-lookup"><span data-stu-id="4d4d1-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="4d4d1-107">Hvis funksjonen ikke er aktivert, kan ikke søkeresultatene hente data fra tidligere datoer.</span><span class="sxs-lookup"><span data-stu-id="4d4d1-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="4d4d1-108">Velg **Aktiviteter,** og finn deretter aktiviteter for **Exchange-postboksen.**</span><span class="sxs-lookup"><span data-stu-id="4d4d1-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="4d4d1-109">Velg **slettede meldinger fra mappen Slettede elementer** og **Flyttede meldinger til mappealternativene Slettede** elementer.</span><span class="sxs-lookup"><span data-stu-id="4d4d1-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="4d4d1-110">Når du er ferdig, klikker du utenfor ruten for å minimere **Aktiviteter-ruten.**</span><span class="sxs-lookup"><span data-stu-id="4d4d1-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="4d4d1-111">Angi datoområdet, og velg **brukernavnet** for brukeren du vil undersøke, i Brukere-boksen.</span><span class="sxs-lookup"><span data-stu-id="4d4d1-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="4d4d1-112">Du kan velge mer enn én bruker om gangen.</span><span class="sxs-lookup"><span data-stu-id="4d4d1-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="4d4d1-113">Velg **Søk.**</span><span class="sxs-lookup"><span data-stu-id="4d4d1-113">Select **Search**.</span></span> <span data-ttu-id="4d4d1-114">Aktivitetene vises under **Resultater.**</span><span class="sxs-lookup"><span data-stu-id="4d4d1-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="4d4d1-115">Hvis du vil vise detaljene, velger du en aktivitet og velger **deretter Mer informasjon.**</span><span class="sxs-lookup"><span data-stu-id="4d4d1-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="4d4d1-116">Tilleggsinformasjon om det slettede elementet, for eksempel emnelinjen og plasseringen av elementet da det ble slettet, vises i **Feltet BerørteElement.**</span><span class="sxs-lookup"><span data-stu-id="4d4d1-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="4d4d1-117">Du kan ikke gjenopprette slettede elementer ved hjelp av funksjonen for overvåkingslogg.</span><span class="sxs-lookup"><span data-stu-id="4d4d1-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="4d4d1-118">Hvis du vil gjenopprette slettede elementer, kan du se [Gjenopprette slettede elementer eller e-post i Outlook Web App.](https://go.microsoft.com/fwlink/?linkid=2103759)</span><span class="sxs-lookup"><span data-stu-id="4d4d1-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="4d4d1-119">Hvis du vil ha mer informasjon, kan du se Søke i overvåkingsloggen for [Office 365 for å feilsøke vanlige scenarioer.](https://go.microsoft.com/fwlink/?linkid=2103944)</span><span class="sxs-lookup"><span data-stu-id="4d4d1-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
