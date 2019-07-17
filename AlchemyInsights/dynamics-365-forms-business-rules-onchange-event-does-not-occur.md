---
title: Dynamics 365 danner forretningsregler - forretningsregel starter ikke i et skjema
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/16/2019
ms.locfileid: "35748273"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange-hendelsen oppstår ikke hvis feltet endres programmatisk

*OnChange* -hendelsen oppstår ikke hvis feltet er endret ved hjelp av *attributt.* [AngiVerdi](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) -metode. Hvis du vil bruke hendelsesbehandlinger for *OnChange* -hendelsen til å kjøre når du har angitt verdien må du bruke den *formContext.data.entity-attributtet.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) -metoden i koden.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
