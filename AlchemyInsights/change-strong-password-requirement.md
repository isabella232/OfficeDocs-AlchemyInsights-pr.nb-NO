---
title: Endre kravet om sterke passord
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: f8790a26ec7c5de57f5dbfc9e1c162767c599f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36518768"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="cfa23-102">Endre kravet om sterke passord</span><span class="sxs-lookup"><span data-stu-id="cfa23-102">Change strong password requirement</span></span>

<span data-ttu-id="cfa23-103">Microsoft krever sterke passord som standard.</span><span class="sxs-lookup"><span data-stu-id="cfa23-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="cfa23-104">Ved hjelp av PowerShell, kan du deaktivere sterke passord for bestemte brukere med denne kommandoen:</span><span class="sxs-lookup"><span data-stu-id="cfa23-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="cfa23-105">*Sett MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="cfa23-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="cfa23-106">Hvis du vil ha mer informasjon om passordpolicyen for</span><span class="sxs-lookup"><span data-stu-id="cfa23-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="cfa23-107">Hvordan du kobler til Office 365 med PowerShell</span><span class="sxs-lookup"><span data-stu-id="cfa23-107">How to connect to Office 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="cfa23-108">Hvis du vil ha mer informasjon om PowerShell MsolUser-kommandoer</span><span class="sxs-lookup"><span data-stu-id="cfa23-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)