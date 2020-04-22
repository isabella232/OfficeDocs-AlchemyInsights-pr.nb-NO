---
title: Feilkode 550 5.7.501 Ingen tilgang, spammisbruk oppdaget
ms.author: chrisda
author: chrisda
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "351"
- "3100015"
ms.assetid: 3105905c-e7a0-42a7-9c5a-61dc56a1d6fc
ms.openlocfilehash: 7be23f02878d12aa08cb4970af6f99539a9cefab
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703035"
---
# <a name="550-57501-access-denied-spam-abuse-detected"></a><span data-ttu-id="c3762-102">550 5.7.501 Ingen tilgang, spammisbruk oppdaget</span><span class="sxs-lookup"><span data-stu-id="c3762-102">550 5.7.501 Access denied, spam abuse detected</span></span>

<span data-ttu-id="c3762-103">Denne meldingen oppstår vanligvis når brukere sender e-postmeldinger fra IP-adresser ved hjelp av det første *onmicrosoft.com* domenet som er tilordnet til nye leiere i Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="c3762-103">Typically, this message occurs when users send email messages from IP addresses using the initial *.onmicrosoft.com* domain that's assigned to new tenants in Microsoft 365.</span></span> <span data-ttu-id="c3762-104">Den enkleste måten å løse dette problemet på, er å:</span><span class="sxs-lookup"><span data-stu-id="c3762-104">The easiest way to resolve this problem is to:</span></span>

1. <span data-ttu-id="c3762-105">[Legg til et domene i leieren](https://docs.microsoft.com//office365/admin/setup/add-domain).</span><span class="sxs-lookup"><span data-stu-id="c3762-105">[Add a domain to your tenant](https://docs.microsoft.com//office365/admin/setup/add-domain).</span></span>

2. <span data-ttu-id="c3762-106">[Endre brukernes primære e-postadresse](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) til det nye egendefinerte domenet du nettopp la til.</span><span class="sxs-lookup"><span data-stu-id="c3762-106">[Change your users' primary email address](https://docs.microsoft.com//office365/admin/add-users/change-a-user-name-and-email-address) to the new custom domain you just added.</span></span>
