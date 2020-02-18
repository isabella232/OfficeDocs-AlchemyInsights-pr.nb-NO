---
title: Koble til MSCommerce-modulen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3529"
ms.openlocfilehash: 80735a03eef6ef9f7b791c43019678ea01f83c00
ms.sourcegitcommit: 9db3be25d088b8d4b2d476aeace79e653ca0a421
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/17/2020
ms.locfileid: "42093604"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a><span data-ttu-id="8d4ae-102">MSCommerce krever en firma- eller faktureringsadministratorkonto</span><span class="sxs-lookup"><span data-stu-id="8d4ae-102">MSCommerce requires a Company or Billing Administrator account</span></span>

<span data-ttu-id="8d4ae-103">MSCommerce-modulen krever en konto med firma- eller faktureringsadministratorrettigheter.</span><span class="sxs-lookup"><span data-stu-id="8d4ae-103">The MSCommerce module requires an account with Company or Billing Administrator privileges.</span></span> <span data-ttu-id="8d4ae-104">Hvis du får følgende feil, må du koble til en annen konto på nytt.</span><span class="sxs-lookup"><span data-stu-id="8d4ae-104">If you are receiving the following error, you will need to reconnect with a different account.</span></span>

    ErrorMessage - The remote server returned an error: (403) Forbidden. ErrorDetails - 
    At C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5
    +     HandleError -ErrorContext $_ -CustomErrorMessage "Failed to retri ...
    +     ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
        + CategoryInfo          : NotSpecified: (:) [Write-Error], WriteErrorException
        + FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError

<span data-ttu-id="8d4ae-105">Hvis kontoen din ikke har rettigheter for firma- eller faktureringsadministrator, kontakter du IT-administratoren.</span><span class="sxs-lookup"><span data-stu-id="8d4ae-105">If your account does not have Company or Billing Administrator privileges, contact your IT Admin.</span></span>
