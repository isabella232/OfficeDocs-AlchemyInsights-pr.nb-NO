---
title: Flere brukere ser ikke tillegg i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197980"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="ad0d1-102">Flere brukere ser ikke tillegg i Outlook</span><span class="sxs-lookup"><span data-stu-id="ad0d1-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="ad0d1-103">Hvis du tester Outlook-tillegg og ingen vises, bruker du cmdleten **Get-OrganizationConfig** PowerShell til å spørre _parameteren AppsForOfficeEnabled_ som første feilsøking.</span><span class="sxs-lookup"><span data-stu-id="ad0d1-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="ad0d1-104">Hvis spørringen returnerer en verdi av **Usann**, setter du denne parameteren til **True** ved hjelp av cmdleten **Set-OrganizationConfig,** slik at tillegg vises som forventet.</span><span class="sxs-lookup"><span data-stu-id="ad0d1-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="ad0d1-105">Vi anbefaler ikke at _parameteren AppsForOfficeEnabled_ er satt til **False**.</span><span class="sxs-lookup"><span data-stu-id="ad0d1-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="ad0d1-106">Verdien **False** overstyrer alle de ovennevnte administrative og brukerrolleinnstillingene og hindrer at nye apper aktiveres av en bruker i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="ad0d1-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="ad0d1-107">Hvis du vil ha mer informasjon, kan du se [Angi administratorer og brukere som kan installere og administrere tillegg for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="ad0d1-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>