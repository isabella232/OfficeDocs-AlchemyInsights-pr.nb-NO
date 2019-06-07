---
title: Opprette og bruke en delt postboks
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762409"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="ec200-102">Feilsøke problemet - brukeren ble ikke funnet i katalogen</span><span class="sxs-lookup"><span data-stu-id="ec200-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="ec200-103">Hvis brukere får feil melding "brukeren finnes ikke" i katalogen.</span><span class="sxs-lookup"><span data-stu-id="ec200-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="ec200-104">Prøv på nytt der problemtypen brukeren ikke er i katalogen.</span><span class="sxs-lookup"><span data-stu-id="ec200-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="ec200-105">Følgende trinn kan fullføres hvis du vil feilsøke problemet.</span><span class="sxs-lookup"><span data-stu-id="ec200-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="ec200-106">Sikre at kontoen som godkjent e-postinvitasjonen er den samme kontoen som brukes til å logge på igjen senere.</span><span class="sxs-lookup"><span data-stu-id="ec200-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="ec200-107">Kontroller at du bruker samme konto til å godta invitasjonen og logge inn på området.</span><span class="sxs-lookup"><span data-stu-id="ec200-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="ec200-108">For mer informasjon, se [å administrere aliaser for Microsoft-kontoen</a> til å administrere Office 365-pålogging](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="ec200-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="ec200-109">Bla til hver område(r) der brukeren mottar feilen.</span><span class="sxs-lookup"><span data-stu-id="ec200-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="ec200-110">Legge til "/ _layouts/15/people.aspx/membershipgroupid=0" (i de doble anførselstegnene) på slutten av URL-adressen for området.</span><span class="sxs-lookup"><span data-stu-id="ec200-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="ec200-111">Eksempel: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="ec200-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="ec200-112">Velg brukeren fra listen.</span><span class="sxs-lookup"><span data-stu-id="ec200-112">Select the user from the list.</span></span>

- <span data-ttu-id="ec200-113">Klikk **Fjern brukertillatelser** fra båndet.</span><span class="sxs-lookup"><span data-stu-id="ec200-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="ec200-114">Legge tilbake til brukeren, og Send invitasjonen på nytt til brukeren.</span><span class="sxs-lookup"><span data-stu-id="ec200-114">Add back the User and Resend the invite to the user.</span></span>

