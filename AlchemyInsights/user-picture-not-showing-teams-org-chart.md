---
title: Brukerbilde vises ikke i Microsoft Teams organisasjonskart
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792760"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Brukerbilde vises ikke i Microsoft Teams organisasjonskart

Hvis én eller flere personer i organisasjonen mangler profilbildet sitt i organisasjonskartet, er det mulig at **Innstillingen ShowInAddressLists** er satt til **False:**

1. Gå til Administrasjonssenter for Microsoft 365 > [**Aktive brukere**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users), og velg brukeren med det manglende bildet. 
1. Velg **E-post-fanen,** og kontroller at **Vis i global adresseliste** er satt til **Ja**. 

Hvis innstillingen **ShowInAddressLists** til **Ja** ikke fungerer, kontrollerer du følgende:

- Brukeren kan være skjult fra mottakerlisten i Exchange. Hvis du vil ha mer informasjon, [kan du se Administrere adresselister i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Brukeren kan være skjult fra adresselisten i Azure Active Directory. Hvis du vil ha mer informasjon, [kan du se Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
