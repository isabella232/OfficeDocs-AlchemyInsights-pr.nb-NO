---
title: Feilsøke et problem – finner ikke brukeren i katalogen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725416"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="cc1d9-102">Feilsøke et problem – finner ikke brukeren i katalogen</span><span class="sxs-lookup"><span data-stu-id="cc1d9-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="cc1d9-103">Hvis brukere får feil meldingen «finner ikke brukeren» i katalogen, kan du prøve på nytt der problem typen er bruker som ikke er i katalog.</span><span class="sxs-lookup"><span data-stu-id="cc1d9-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="cc1d9-104">Følgende trinn kan utføres for å feilsøke problemet.</span><span class="sxs-lookup"><span data-stu-id="cc1d9-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="cc1d9-105">Kontroller at kontoen som godtok e-postinvitasjonen, er den samme kontoen som brukes til å logge på senere.</span><span class="sxs-lookup"><span data-stu-id="cc1d9-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="cc1d9-106">Kontroller at brukeren bruker samme konto til å godta invitasjonen og logge på nettstedet.</span><span class="sxs-lookup"><span data-stu-id="cc1d9-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="cc1d9-107">Hvis du vil ha mer informasjon, kan du se [hvordan du behandler aliaser for Microsoft-kontoen for </a> å administrere Microsoft 365-påloggingen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="cc1d9-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="cc1d9-108">Gå til hvert område (r) som brukeren mottar feilen i.</span><span class="sxs-lookup"><span data-stu-id="cc1d9-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="cc1d9-109">Legg til «/_layouts/15/People.aspx/membershipgroupid = 0» (i doble anførsels tegn) på slutten av Netta dressen for nettstedet.</span><span class="sxs-lookup"><span data-stu-id="cc1d9-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="cc1d9-110">Eksempel: https://< «contoso» >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="cc1d9-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="cc1d9-111">Velg brukeren fra listen.</span><span class="sxs-lookup"><span data-stu-id="cc1d9-111">Select the user from the list.</span></span>

- <span data-ttu-id="cc1d9-112">Klikk **Fjern bruker tillatelser** fra båndet.</span><span class="sxs-lookup"><span data-stu-id="cc1d9-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="cc1d9-113">Legg tilbake brukeren og Send invitasjonen til brukeren på nytt.</span><span class="sxs-lookup"><span data-stu-id="cc1d9-113">Add back the User and Resend the invite to the user.</span></span>

