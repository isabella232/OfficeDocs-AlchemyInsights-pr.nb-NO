---
title: Identifisere innboksen regelen aktivitet i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909422"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="2e90c-102">Identifisere innboksen regelen aktivitet i overvåkingslogger</span><span class="sxs-lookup"><span data-stu-id="2e90c-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="2e90c-103">Du kan bruke sporing Logg Søk i Security-& overholdelsessenteret for å vise innboksen regelen hendelser (opprette, endre og slette innboksregler).</span><span class="sxs-lookup"><span data-stu-id="2e90c-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="2e90c-104">Logg på [Office 365 & kompatibilitet Sikkerhetssenter](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="2e90c-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="2e90c-105">Klikk **Søk og undersøkelser** , og velg **Overvåk Logg Søk**.</span><span class="sxs-lookup"><span data-stu-id="2e90c-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="2e90c-106">Velg datointervallet i feltene **Startdato** og **Sluttdato** .</span><span class="sxs-lookup"><span data-stu-id="2e90c-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="2e90c-107">Under **Aktiviteter for Exchange-postboksen**, kan du kontrollere **aktiviteter** -feltet er satt til **Ny-InboxRule-Opprett/endre/aktivere/deaktivere Innboksregel**.</span><span class="sxs-lookup"><span data-stu-id="2e90c-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="2e90c-108">Klikk **Søk**.</span><span class="sxs-lookup"><span data-stu-id="2e90c-108">Click **Search**.</span></span>

<span data-ttu-id="2e90c-109">I resultatene, velger du et kontrollregister.</span><span class="sxs-lookup"><span data-stu-id="2e90c-109">In the results, select an audit record.</span></span> <span data-ttu-id="2e90c-110">Klikk **Mer informasjon**i detaljer-undermeny.</span><span class="sxs-lookup"><span data-stu-id="2e90c-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="2e90c-111">Informasjon om innstillingene i innboksen vises i **Parametere** -feltet.</span><span class="sxs-lookup"><span data-stu-id="2e90c-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="2e90c-112">Hvis du vil ha mer informasjon, se [Determining Hvis en bruker opprettet en regel](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="2e90c-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
