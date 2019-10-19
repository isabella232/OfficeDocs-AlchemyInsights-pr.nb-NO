---
title: Dynamics 365 skjemaer forretningsregler-forretningsregel utløses ikke for et skjema
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36529028"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="e77bf-102">OnChange-hendelsen oppstår ikke hvis feltet endres programmatisk</span><span class="sxs-lookup"><span data-stu-id="e77bf-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="e77bf-103">*OnChange* -hendelsen oppstår ikke hvis feltet endres programmatisk ved hjelp av *attributtet.* [Angi verdi](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metode.</span><span class="sxs-lookup"><span data-stu-id="e77bf-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="e77bf-104">Hvis du vil at hendelsesbehandlinger for hendelsen *OnChange* skal kjøres etter at du har angitt verdien, må du bruke *attributtet formContext. data. Entity.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) -metoden i koden.</span><span class="sxs-lookup"><span data-stu-id="e77bf-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
