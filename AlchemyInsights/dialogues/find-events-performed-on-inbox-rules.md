---
title: Finne hendelser som utføres på innboksregler
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430011"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="34b92-102">Finne hendelser som utføres på innboksregler</span><span class="sxs-lookup"><span data-stu-id="34b92-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="34b92-103">Når innboksregler opprettes, endres eller slettes, registreres hendelsene i overvåkingsloggen.</span><span class="sxs-lookup"><span data-stu-id="34b92-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="34b92-104">Slik ser du gjennom dem:</span><span class="sxs-lookup"><span data-stu-id="34b92-104">Here's how to review them:</span></span>

1. <span data-ttu-id="34b92-105">Gå til [sikkerhetssenteret for Office 365 &.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="34b92-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="34b92-106">Velg Søk > søk i overvåkingsloggen.</span><span class="sxs-lookup"><span data-stu-id="34b92-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="34b92-107">Hvis du ser en melding om at du må aktivere overvåking, går du videre og slår den på nå.</span><span class="sxs-lookup"><span data-stu-id="34b92-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="34b92-108">Hvis denne funksjonen ikke er aktivert, kan ikke søkeresultatene hente data fra tidligere datoer.</span><span class="sxs-lookup"><span data-stu-id="34b92-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="34b92-109">Velg Aktiviteter-feltet og finn aktiviteter for Exchange-postboksen, og velg deretter New-InboxRule Opprett innboksregel fra Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="34b92-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="34b92-110">Når du er ferdig, klikker du utenfor ruten for å minimere Aktiviteter-ruten.</span><span class="sxs-lookup"><span data-stu-id="34b92-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="34b92-111">Angi datoområdet, og velg brukernavnet for brukeren du vil undersøke, i Brukere-feltet.</span><span class="sxs-lookup"><span data-stu-id="34b92-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="34b92-112">Du kan velge mer enn én bruker om gangen.</span><span class="sxs-lookup"><span data-stu-id="34b92-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="34b92-113">Velg Søk.</span><span class="sxs-lookup"><span data-stu-id="34b92-113">Select Search.</span></span> <span data-ttu-id="34b92-114">Aktivitetene vises under Resultater.</span><span class="sxs-lookup"><span data-stu-id="34b92-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="34b92-115">Hvis du vil vise detaljer, velger du en aktivitet og velger deretter Mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="34b92-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="34b92-116">Under Parametere-delen kan du se navnet på regelen, betingelsene som er angitt, og handlingene regelen vil utføre.</span><span class="sxs-lookup"><span data-stu-id="34b92-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="34b92-117">Hvis du vil ha mer informasjon, kan du se Søke i overvåkingsloggen for Office 365 for å feilsøke vanlige scenarier.</span><span class="sxs-lookup"><span data-stu-id="34b92-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>