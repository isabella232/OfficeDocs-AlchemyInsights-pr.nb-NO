---
title: Feilsøking av problem-brukeren ikke funnet i katalogen
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754201"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="dc258-102">Feilsøking av problem-brukeren ikke funnet i katalogen</span><span class="sxs-lookup"><span data-stu-id="dc258-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="dc258-103">Hvis brukere får feilmeldingen "brukeren kan ikke finnes" i katalogen.</span><span class="sxs-lookup"><span data-stu-id="dc258-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="dc258-104">Behage prøve atter der hvor utsendelsen type er bruker ikke inne adresseliste.</span><span class="sxs-lookup"><span data-stu-id="dc258-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="dc258-105">Følgende trinn kan fullføres for å feilsøke problemet.</span><span class="sxs-lookup"><span data-stu-id="dc258-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="dc258-106">Kontroller at kontoen som godtok invitasjonen til e-post, er den samme kontoen som brukes til å logge på senere.</span><span class="sxs-lookup"><span data-stu-id="dc258-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="dc258-107">Kontroller at brukeren bruker samme konto til å godta invitasjonen og logge på området.</span><span class="sxs-lookup"><span data-stu-id="dc258-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="dc258-108">Hvis du vil ha mer informasjon, kan du se Administrere [aliaser for</a> Microsoft-kontoen din for å administrere Office 365-påloggingen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="dc258-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="dc258-109">Bla til hvert område (r) der brukeren mottar feilen.</span><span class="sxs-lookup"><span data-stu-id="dc258-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="dc258-110">Legg til "/_layouts/15/People.aspx/membershipgroupid = 0" (i doble anførselstegn) til slutten av webadressen.</span><span class="sxs-lookup"><span data-stu-id="dc258-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="dc258-111">Eksempel: https://< "contoso">. SharePoint. com/layouts/15/People. aspx/membershipGroupId = 0.</span><span class="sxs-lookup"><span data-stu-id="dc258-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="dc258-112">Velg brukeren fra listen.</span><span class="sxs-lookup"><span data-stu-id="dc258-112">Select the user from the list.</span></span>

- <span data-ttu-id="dc258-113">Klikk **Fjern brukertillatelser** fra båndet.</span><span class="sxs-lookup"><span data-stu-id="dc258-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="dc258-114">Legg til brukeren og Send invitasjonen til brukeren på nytt.</span><span class="sxs-lookup"><span data-stu-id="dc258-114">Add back the User and Resend the invite to the user.</span></span>

