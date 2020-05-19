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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/27/2020
ms.locfileid: "44282929"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a><span data-ttu-id="c8c1d-102">Endre e-postadressen til en Microsoft 365-gruppe</span><span class="sxs-lookup"><span data-stu-id="c8c1d-102">Change email address of an Microsoft 365 group</span></span>

<span data-ttu-id="c8c1d-103">Du kan endre e-postadressen til en Microsoft 365-gruppe ved hjelp av administrasjonssenteret.</span><span class="sxs-lookup"><span data-stu-id="c8c1d-103">You can change the email address of an Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="c8c1d-104">Bare velg gruppen og velg @edit e-postadresse.</span><span class="sxs-lookup"><span data-stu-id="c8c1d-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="c8c1d-105">Du kan også bruke følgende EXO PowerShell-kommandoen til å endre den primære SMTP-adressen til en Microsoft 365-gruppe:</span><span class="sxs-lookup"><span data-stu-id="c8c1d-105">You can also use following the EXO PowerShell command to change the primary SMTP address of an Microsoft 365 group:</span></span>

<span data-ttu-id="c8c1d-106">Angi UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="c8c1d-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="c8c1d-107">Eksempel:</span><span class="sxs-lookup"><span data-stu-id="c8c1d-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
