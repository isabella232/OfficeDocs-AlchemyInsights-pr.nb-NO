---
title: Identifisere regel aktivitet for innboksen i overvåkings logger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779060"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="0ba7f-102">Identifisere regel aktivitet for innboksen i overvåkings logger</span><span class="sxs-lookup"><span data-stu-id="0ba7f-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="0ba7f-103">Du kan bruke overvåkings Logg søk i 365 Microsofts sikkerhets & Samsvars senter for å vise regel hendelser for innboksen (oppretting, endring og sletting av regler for innboksen).</span><span class="sxs-lookup"><span data-stu-id="0ba7f-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="0ba7f-104">Logg på [sikkerhets & samsvars senteret til Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="0ba7f-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="0ba7f-105">Gå til **Search**  >  **søke siden for overvåkings Logg** for søk.</span><span class="sxs-lookup"><span data-stu-id="0ba7f-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="0ba7f-106">Velg dato området i feltene **Start dato** og **slutt dato** .</span><span class="sxs-lookup"><span data-stu-id="0ba7f-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="0ba7f-107">Under **Exchange post boks aktiviteter**kontrollerer du at **aktiviteter** -feltet er satt til **New-InboxRule Create/modify/enable/disable Rule**.</span><span class="sxs-lookup"><span data-stu-id="0ba7f-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="0ba7f-108">Klikk **Søk**.</span><span class="sxs-lookup"><span data-stu-id="0ba7f-108">Click **Search**.</span></span>

<span data-ttu-id="0ba7f-109">Velg en overvåkings post i resultatene.</span><span class="sxs-lookup"><span data-stu-id="0ba7f-109">In the results, select an audit record.</span></span> <span data-ttu-id="0ba7f-110">Klikk **mer informasjon**i under menyen detaljer.</span><span class="sxs-lookup"><span data-stu-id="0ba7f-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="0ba7f-111">Informasjon om innstillingene for innboks-regelen vises i **Parametere** -feltet.</span><span class="sxs-lookup"><span data-stu-id="0ba7f-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="0ba7f-112">Hvis du vil ha mer informasjon, kan du se [fastslå om en bruker har opprettet en innboks-regel](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="0ba7f-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
