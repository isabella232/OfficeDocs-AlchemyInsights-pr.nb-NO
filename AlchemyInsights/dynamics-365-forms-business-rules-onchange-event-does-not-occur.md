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
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769348"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="6cf08-102">OnChange-hendelsen oppstår ikke hvis feltet endres programmatisk</span><span class="sxs-lookup"><span data-stu-id="6cf08-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="6cf08-103">*OnChange* -hendelsen oppstår ikke hvis feltet endres programmatisk ved hjelp av *attributtet.* [Angi verdi](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metode.</span><span class="sxs-lookup"><span data-stu-id="6cf08-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="6cf08-104">Hvis du vil at hendelsesbehandlinger for *OnChange* -hendelsen skal kjøres etter at du har angitt verdien, må du bruke *formContext. data. Entity-attributtet* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) i koden.</span><span class="sxs-lookup"><span data-stu-id="6cf08-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
