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
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="b976d-102">Flere brukere får ingen tilgangsfeil mens du legger til tillegg i Outlook</span><span class="sxs-lookup"><span data-stu-id="b976d-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="b976d-103">Du kan angi hvilke administratorer i organisasjonen som har tillatelse til å installere og administrere tillegg for Outlook.</span><span class="sxs-lookup"><span data-stu-id="b976d-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="b976d-104">Du kan også angi hvilke brukere i organisasjonen som har tillatelse til å installere og administrere tillegg for eget bruk.</span><span class="sxs-lookup"><span data-stu-id="b976d-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="b976d-105">Hvis du vil ha mer informasjon, kan du se [Angi administratorer og brukere som kan installere og administrere tillegg for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="b976d-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="b976d-106">Hvis du vil kontrollere at du har tilordnet tillatelser for en bruker, erstatter du <Role Name> med navnet på rollen som skal kontrolleres, og kjører følgende kommando i Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="b976d-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="b976d-107">Get-ManagementRoleAssignment -Rolle " <Role Name> " -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="b976d-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="b976d-108">Dette eksemplet viser deg hvordan du kontrollerer hvem du har tilordnet tillatelser til å installere tillegg fra Office Store for organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="b976d-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="b976d-109">Powershell</span><span class="sxs-lookup"><span data-stu-id="b976d-109">PowerShell</span></span>

<span data-ttu-id="b976d-110">-Rolle "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="b976d-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="b976d-111">Se gjennom oppføringene i kolonnen Effektive brukere i resultatene.</span><span class="sxs-lookup"><span data-stu-id="b976d-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="b976d-112">Hvis du vil ha detaljert syntaks- og parameterinformasjon, kan du se [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="b976d-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 