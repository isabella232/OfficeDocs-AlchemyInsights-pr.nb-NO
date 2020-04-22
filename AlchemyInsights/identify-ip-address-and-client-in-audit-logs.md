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
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716397"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="579bc-102">Identifisere IP-adresse og klient i overvåkingslogger</span><span class="sxs-lookup"><span data-stu-id="579bc-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="579bc-103">IP-adressen som tilsvarer en aktivitet av en Microsoft 365-bruker eller administrator, vises i overvåkingsloggene.</span><span class="sxs-lookup"><span data-stu-id="579bc-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="579bc-104">Klientinformasjonen logges også.</span><span class="sxs-lookup"><span data-stu-id="579bc-104">The client information is also logged.</span></span> <span data-ttu-id="579bc-105">Her er fremgangsmåten for å identifisere slik informasjon</span><span class="sxs-lookup"><span data-stu-id="579bc-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="579bc-106">Logg på [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="579bc-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="579bc-107">Gå til**søkesiden for søkeloggen for søke etter** søk i **søkesiden for søkeetter søk.** > </span><span class="sxs-lookup"><span data-stu-id="579bc-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="579bc-108">Hvis du er interessert i en bestemt aktivitet, velger du den fra **Aktivitetsliste.**</span><span class="sxs-lookup"><span data-stu-id="579bc-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="579bc-109">Hvis ikke, returneres alle aktiviteter for den valgte brukeren (standardinnstilling).</span><span class="sxs-lookup"><span data-stu-id="579bc-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="579bc-110">**Merk:** Enkelte aktiviteter er kanskje ikke tilgjengelige i **Aktiviteter-menyen.** Disse overvåkingselementene returneres imidlertid hvis **Vis resultater for alle aktiviteter** er valgt (standardinnstilling).</span><span class="sxs-lookup"><span data-stu-id="579bc-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="579bc-111">Angi brukernavnet i **Brukere-feltet,** velg riktig datoperiode for aktiviteten, og klikk deretter **Søk**.</span><span class="sxs-lookup"><span data-stu-id="579bc-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="579bc-112">I resultatene kan du se IP-adressen for denne aktiviteten i resultatruten.</span><span class="sxs-lookup"><span data-stu-id="579bc-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="579bc-113">Velg overvåkingsoppføringen for å se detaljert informasjon i **undermenyen Detaljer** (for eksempel Klient, Bruker som utførte handlingen osv.).</span><span class="sxs-lookup"><span data-stu-id="579bc-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="579bc-114">Hvis du vil ha mer informasjon, kan du se [Finne IP-adressen til datamaskinen som brukes til å få tilgang til en kompromittert konto](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="579bc-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
