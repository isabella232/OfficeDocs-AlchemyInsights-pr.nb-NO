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
# <a name="change-strong-password-requirement"></a>Endre kravet om sterke passord

Microsoft krever sterke passord som standard. 

Ved hjelp av PowerShell, kan du deaktivere sterke passord for bestemte brukere med denne kommandoen:<br>
*Sett MsolUser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [Hvis du vil ha mer informasjon om passordpolicyen for](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Hvordan du kobler til Office 365 med PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Hvis du vil ha mer informasjon om PowerShell MsolUser-kommandoer](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)