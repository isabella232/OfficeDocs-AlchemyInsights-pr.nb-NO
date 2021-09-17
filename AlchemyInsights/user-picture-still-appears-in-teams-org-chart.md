---
title: Brukerbilde vises fremdeles i Microsoft Teams organisasjonskartet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422248"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Brukerbilde vises fremdeles i Microsoft Teams organisasjonskartet

Hvis én eller flere personer i organisasjonen har blitt deaktivert eller fjernet, og profilbildet fremdeles vises i organisasjonskartet, er det mulig innstillingen **ShowInAddressLists** er satt til False: 

1. Gå til Administrasjonssenter for Microsoft 365 > [Aktive brukere,](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) og velg brukeren med bildet som fremdeles vises. 
1. Velg **E-post-fanen,** og kontroller at **Vis i global adresseliste** er satt til **Nei**.

Hvis innstillingen **ShowInAddressLists** til **Nei** ikke fungerer, kontrollerer du følgende: 

- Brukeren kan vises fra mottakerlisten i Exchange. Hvis du vil ha mer informasjon, [kan du se Administrere adresselister i Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Brukeren kan vises fra adresselisten i Azure Active Directory. Hvis du vil ha mer informasjon, [kan du se Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 