---
title: Endre e-postadressen til en Microsoft 365-gruppe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580666"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="5197b-102">Endre e-postadressen til en Microsoft 365-gruppe</span><span class="sxs-lookup"><span data-stu-id="5197b-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="5197b-103">Du kan endre e-postadressen til en Microsoft 365-gruppe ved hjelp av administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="5197b-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="5197b-104">Bare velg gruppen og velg @edit e-postadresse.</span><span class="sxs-lookup"><span data-stu-id="5197b-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="5197b-105">Du kan også bruke følgende EXO PowerShell -kommandoen til å endre den primære SMTP-adressen til en Microsoft 365-gruppe:</span><span class="sxs-lookup"><span data-stu-id="5197b-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="5197b-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="5197b-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="5197b-107">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="5197b-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
