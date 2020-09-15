---
title: Identifisere IP-adresse og klient i overvåkings logger
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668319"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="24c7e-102">Identifisere IP-adresse og klient i overvåkings logger</span><span class="sxs-lookup"><span data-stu-id="24c7e-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="24c7e-103">IP-adressen som tilsvarer en aktivitet av en Microsoft 365-bruker eller-administrator, vises i overvåkings loggene.</span><span class="sxs-lookup"><span data-stu-id="24c7e-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="24c7e-104">Klient informasjonen er også logget.</span><span class="sxs-lookup"><span data-stu-id="24c7e-104">The client information is also logged.</span></span> <span data-ttu-id="24c7e-105">Her er Fremgangs måten for å identifisere denne informasjonen</span><span class="sxs-lookup"><span data-stu-id="24c7e-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="24c7e-106">Logg på [sikkerhets & samsvars senteret til Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="24c7e-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="24c7e-107">Gå til **Search**  >  **søke siden for overvåkings Logg** for søk.</span><span class="sxs-lookup"><span data-stu-id="24c7e-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="24c7e-108">Hvis du er interessert i en bestemt aktivitet, velger du den fra **aktiviteter** -listen.</span><span class="sxs-lookup"><span data-stu-id="24c7e-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="24c7e-109">Hvis ikke, blir alle aktiviteter returnert for den valgte brukeren (standard innstilling).</span><span class="sxs-lookup"><span data-stu-id="24c7e-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="24c7e-110">**Obs**! visse aktiviteter er kanskje ikke tilgjengelige i **aktiviteter** -menyen. disse overvåkings elementene blir imidlertid returnert Hvis **Vis resultater for alle aktiviteter** er valgt (standard innstilling).</span><span class="sxs-lookup"><span data-stu-id="24c7e-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="24c7e-111">Angi bruker navnet i **brukere** -feltet, Velg det aktuelle dato intervallet for aktiviteten, og klikk deretter **Søk**.</span><span class="sxs-lookup"><span data-stu-id="24c7e-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="24c7e-112">I resultatene kan du se IP-adressen for denne aktiviteten i Resultater-ruten.</span><span class="sxs-lookup"><span data-stu-id="24c7e-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="24c7e-113">Velg overvåkings posten for å se detaljert informasjon i **detaljer** -undermenyen (for eksempel klient, bruker som utførte handlinger osv.).</span><span class="sxs-lookup"><span data-stu-id="24c7e-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="24c7e-114">Hvis du vil ha mer informasjon, kan du se [finne IP-adressen til data maskinen som brukes til å få tilgang til en kompromittert konto](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="24c7e-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
