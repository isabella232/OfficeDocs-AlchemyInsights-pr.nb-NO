---
title: Identifisere innboksregelaktivitet i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716433"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="068e1-102">Identifisere innboksregelaktivitet i overvåkingslogger</span><span class="sxs-lookup"><span data-stu-id="068e1-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="068e1-103">Du kan bruke overvåkingsloggsøk i Microsoft 365 Security & Compliance Center til å vise regler for innboksregel (opprette, endre og slette innboksregler).</span><span class="sxs-lookup"><span data-stu-id="068e1-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="068e1-104">Logg på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="068e1-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="068e1-105">Gå til**søkesiden for søkeloggen for søke etter** søk i **søkesiden for søkeetter søk.** > </span><span class="sxs-lookup"><span data-stu-id="068e1-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="068e1-106">Velg datoperioden i feltene **Startdato** og **Sluttdato.**</span><span class="sxs-lookup"><span data-stu-id="068e1-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="068e1-107">Under **Exchange-postboksaktiviteter**kontrollerer du **aktiviteter-feltet** er satt til **Ny-inboxRule Opprett/endre/aktivere/deaktivere innboksregel**.</span><span class="sxs-lookup"><span data-stu-id="068e1-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="068e1-108">Klikk **Søk**.</span><span class="sxs-lookup"><span data-stu-id="068e1-108">Click **Search**.</span></span>

<span data-ttu-id="068e1-109">Velg en overvåkingspost i resultatene.</span><span class="sxs-lookup"><span data-stu-id="068e1-109">In the results, select an audit record.</span></span> <span data-ttu-id="068e1-110">Klikk **Mer informasjon**i undermenyen for detaljer.</span><span class="sxs-lookup"><span data-stu-id="068e1-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="068e1-111">Informasjon om innboksregelinnstillingene vises i **Parametere-feltet.**</span><span class="sxs-lookup"><span data-stu-id="068e1-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="068e1-112">Hvis du vil ha mer informasjon, kan du se [Finne ut om en bruker opprettet en innboksregel](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="068e1-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
