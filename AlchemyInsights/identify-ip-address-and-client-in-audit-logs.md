---
title: Identifisere IP-adressen og klient i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539038"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="0cf66-102">Identifisere IP-adressen og klient i overvåkingslogger</span><span class="sxs-lookup"><span data-stu-id="0cf66-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="0cf66-103">IP-adresse som svarer til en aktivitet med en Office 365-bruker eller administrator vises i overvåkingsloggen.</span><span class="sxs-lookup"><span data-stu-id="0cf66-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="0cf66-104">Informasjon om klient logges også.</span><span class="sxs-lookup"><span data-stu-id="0cf66-104">The client information is also logged.</span></span> <span data-ttu-id="0cf66-105">Her er fremgangsmåten for å identifisere slike opplysninger</span><span class="sxs-lookup"><span data-stu-id="0cf66-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="0cf66-106">Logg på [Office 365 & kompatibilitet Sikkerhetssenter](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="0cf66-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="0cf66-107">Gå til **Søk** > **Overvåk Logg Søk** -siden.</span><span class="sxs-lookup"><span data-stu-id="0cf66-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="0cf66-108">Hvis du er interessert i en bestemt aktivitet, kan du velge den fra **aktiviteter** -listen.</span><span class="sxs-lookup"><span data-stu-id="0cf66-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="0cf66-109">Hvis ikke, returneres alle aktiviteter for den valgte brukeren (standardinnstilling).</span><span class="sxs-lookup"><span data-stu-id="0cf66-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="0cf66-110">**Merk**: enkelte aktiviteter er kanskje ikke tilgjengelig i **aktiviteter** -menyen. imidlertid de overvåke varer returneres hvis **Vise resultater for alle aktiviteter som** er valgt (standardinnstillingen).</span><span class="sxs-lookup"><span data-stu-id="0cf66-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="0cf66-111">Angi brukernavnet i **brukere** -feltet, velg riktig datointervallet for aktiviteten og deretter **Søk**.</span><span class="sxs-lookup"><span data-stu-id="0cf66-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="0cf66-112">I resultatene, kan du se IP-adressen for denne aktiviteten i resultater-ruten.</span><span class="sxs-lookup"><span data-stu-id="0cf66-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="0cf66-113">Velg kontrollregister å se detaljert informasjon i **Detaljer** -undermeny (for eksempel klient, brukeren som utførte handlingen, osv.).</span><span class="sxs-lookup"><span data-stu-id="0cf66-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="0cf66-114">Hvis du vil ha mer informasjon, kan du se [finne IP-adressen til datamaskinen for å få tilgang til et utsatt konto](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="0cf66-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
