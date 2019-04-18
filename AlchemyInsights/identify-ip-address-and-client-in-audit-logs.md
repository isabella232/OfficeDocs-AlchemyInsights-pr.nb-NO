---
title: Identifisere IP-adressen og klient i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909423"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="8ce65-102">Identifisere IP-adressen og klient i overvåkingslogger</span><span class="sxs-lookup"><span data-stu-id="8ce65-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="8ce65-103">IP-adressen som samsvarer med en aktivitet etter en bruker eller administrator vises i overvåkingsloggen.</span><span class="sxs-lookup"><span data-stu-id="8ce65-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="8ce65-104">Informasjon om klient logges også.</span><span class="sxs-lookup"><span data-stu-id="8ce65-104">The client information is also logged.</span></span> <span data-ttu-id="8ce65-105">Her er fremgangsmåten for å identifisere slike opplysninger</span><span class="sxs-lookup"><span data-stu-id="8ce65-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="8ce65-106">Logg på [Office 365 & kompatibilitet Sikkerhetssenter](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="8ce65-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="8ce65-107">Klikk **Søk og undersøkelser** , og velg **Overvåk Logg Søk**.</span><span class="sxs-lookup"><span data-stu-id="8ce65-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="8ce65-108">Hvis du er interessert i en bestemt aktivitet, kan du velge den fra **aktiviteter** -listen.</span><span class="sxs-lookup"><span data-stu-id="8ce65-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="8ce65-109">Hvis ikke, returneres alle aktiviteter for den valgte brukeren (standardinnstilling).</span><span class="sxs-lookup"><span data-stu-id="8ce65-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="8ce65-110">**Merk**: enkelte aktiviteter er kanskje ikke tilgjengelig i **aktiviteter** -menyen. imidlertid de overvåke varer returneres hvis **Vise resultater for alle aktiviteter som** er valgt (standardinnstillingen).</span><span class="sxs-lookup"><span data-stu-id="8ce65-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="8ce65-111">Angi brukernavnet i **brukere** -feltet, velg riktig datointervallet for aktiviteten og deretter **Søk**.</span><span class="sxs-lookup"><span data-stu-id="8ce65-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="8ce65-112">I resultatene, kan du se IP-adressen for denne aktiviteten i resultater-ruten.</span><span class="sxs-lookup"><span data-stu-id="8ce65-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="8ce65-113">Velg kontrollregister å se detaljert informasjon i **Detaljer** -undermeny (for eksempel klient, brukeren som utførte handlingen, osv.).</span><span class="sxs-lookup"><span data-stu-id="8ce65-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="8ce65-114">Hvis du vil ha mer informasjon, kan du se [finne IP-adressen til datamaskinen for å få tilgang til et utsatt konto](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="8ce65-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
