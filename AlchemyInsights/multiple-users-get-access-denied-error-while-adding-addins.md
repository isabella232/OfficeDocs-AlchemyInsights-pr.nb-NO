---
title: Flere brukere får ingen tilgangsfeil mens du legger til tillegg i Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424169"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Flere brukere får ingen tilgangsfeil mens du legger til tillegg i Outlook

Du kan angi hvilke administratorer i organisasjonen som har tillatelse til å installere og administrere tillegg for Outlook. Du kan også angi hvilke brukere i organisasjonen som har tillatelse til å installere og administrere tillegg for eget bruk.

Hvis du vil ha mer informasjon, kan du se [Angi administratorer og brukere som kan installere og administrere tillegg for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Hvis du vil kontrollere at du har tilordnet tillatelser for en bruker, erstatter du <Role Name> med navnet på rollen som skal kontrolleres, og kjører følgende kommando i Exchange Online PowerShell:

Get-ManagementRoleAssignment -Rolle " <Role Name> " -GetEffectiveUsers

Dette eksemplet viser deg hvordan du kontrollerer hvem du har tilordnet tillatelser til å installere tillegg fra Office Store for organisasjonen.

Powershell

-Rolle "Org Marketplace Apps" -GetEffectiveUsers

Se gjennom oppføringene i kolonnen Effektive brukere i resultatene.

Hvis du vil ha detaljert syntaks- og parameterinformasjon, kan du se [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 