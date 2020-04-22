---
title: Feilsøke problem - Finner ikke brukeren i katalogen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702747"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="81590-102">Feilsøke problem - Finner ikke brukeren i katalogen</span><span class="sxs-lookup"><span data-stu-id="81590-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="81590-103">Hvis brukere mottar feilmeldingen "finner ikke brukeren" i katalogen, kan du prøve på nytt der problemtypen ikke er bruker i katalogen.</span><span class="sxs-lookup"><span data-stu-id="81590-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="81590-104">Følgende trinn kan fullføres for å feilsøke problemet.</span><span class="sxs-lookup"><span data-stu-id="81590-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="81590-105">Kontroller at kontoen som godtok e-postinvitasjonen, er den samme kontoen som brukes til å logge på senere.</span><span class="sxs-lookup"><span data-stu-id="81590-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="81590-106">Kontroller at brukeren bruker den samme kontoen til å godta invitasjonen og logge på nettstedet.</span><span class="sxs-lookup"><span data-stu-id="81590-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="81590-107">Hvis du vil ha mer informasjon, kan du se [Administrere aliaser for Microsoft-kontoen</a> for å administrere Microsoft 365-påloggingen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="81590-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="81590-108">Bla til hvert område(er) der brukeren mottar feilen.</span><span class="sxs-lookup"><span data-stu-id="81590-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="81590-109">Legg til "/_layouts/15/people.aspx/membershipgroupid=0" (innenfor de doble anførselstegn) på slutten av url-adressen for området.</span><span class="sxs-lookup"><span data-stu-id="81590-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="81590-110">Eksempel: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="81590-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="81590-111">Velg brukeren fra listen.</span><span class="sxs-lookup"><span data-stu-id="81590-111">Select the user from the list.</span></span>

- <span data-ttu-id="81590-112">Klikk **Fjern brukertillatelser** fra båndet.</span><span class="sxs-lookup"><span data-stu-id="81590-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="81590-113">Legg til brukeren på nytt, og send invitasjonen til brukeren på nytt.</span><span class="sxs-lookup"><span data-stu-id="81590-113">Add back the User and Resend the invite to the user.</span></span>

