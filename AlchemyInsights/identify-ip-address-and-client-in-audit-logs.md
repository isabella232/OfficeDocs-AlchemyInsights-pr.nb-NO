---
title: Identifisere IP-adresse og klient i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508925"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="bc9f8-102">Identifisere IP-adresse og klient i overvåkingslogger</span><span class="sxs-lookup"><span data-stu-id="bc9f8-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="bc9f8-103">IP-adressen som tilsvarer en aktivitet av en Microsoft 365-bruker eller administrator, vises i overvåkingsloggene.</span><span class="sxs-lookup"><span data-stu-id="bc9f8-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="bc9f8-104">Klientinformasjonen logges også.</span><span class="sxs-lookup"><span data-stu-id="bc9f8-104">The client information is also logged.</span></span> <span data-ttu-id="bc9f8-105">Her er fremgangsmåten for å identifisere slik informasjon</span><span class="sxs-lookup"><span data-stu-id="bc9f8-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="bc9f8-106">Logg på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="bc9f8-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="bc9f8-107">Gå til søkeloggen for søk i **søkeloggen for søk i søkeloggen for søk**  >  **Audit log search** i søke.</span><span class="sxs-lookup"><span data-stu-id="bc9f8-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="bc9f8-108">Hvis du er interessert i en bestemt aktivitet, velger du den fra **Aktiviteter-listen.**</span><span class="sxs-lookup"><span data-stu-id="bc9f8-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="bc9f8-109">Hvis ikke, returneres alle aktiviteter for den valgte brukeren (standardinnstillingen).</span><span class="sxs-lookup"><span data-stu-id="bc9f8-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="bc9f8-110">**Merk:** Enkelte aktiviteter er kanskje ikke tilgjengelige i **Aktiviteter-menyen.** Disse overvåkingselementene returneres imidlertid hvis **Vis resultater for alle aktiviteter** er valgt (standardinnstilling).</span><span class="sxs-lookup"><span data-stu-id="bc9f8-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="bc9f8-111">Angi brukernavnet i **Brukere-feltet,** velg riktig datoperiode for aktiviteten, og klikk deretter **Søk**.</span><span class="sxs-lookup"><span data-stu-id="bc9f8-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="bc9f8-112">I resultatene kan du se IP-adressen for denne aktiviteten i resultatruten.</span><span class="sxs-lookup"><span data-stu-id="bc9f8-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="bc9f8-113">Velg overvåkingsoppføringen for å se detaljert informasjon i **undermenyen Detaljer** (for eksempel Klient, Bruker som utførte handling osv.).</span><span class="sxs-lookup"><span data-stu-id="bc9f8-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="bc9f8-114">Hvis du vil ha mer informasjon, kan du se [Finne IP-adressen til datamaskinen som brukes til å få tilgang til en kompromittert konto](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="bc9f8-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
