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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769348"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange-hendelsen oppstår ikke hvis feltet endres programmatisk

*OnChange* -hendelsen oppstår ikke hvis feltet endres programmatisk ved hjelp av *attributtet.* [Angi verdi](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) metode. Hvis du vil at hendelsesbehandlinger for *OnChange* -hendelsen skal kjøres etter at du har angitt verdien, må du bruke *formContext. data. Entity-attributtet* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) i koden.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
