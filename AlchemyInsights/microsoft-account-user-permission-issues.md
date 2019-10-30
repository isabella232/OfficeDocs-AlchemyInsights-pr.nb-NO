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
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768810"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="a9450-102">Feilsøking av problem-brukeren ikke funnet i katalogen</span><span class="sxs-lookup"><span data-stu-id="a9450-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="a9450-103">Hvis brukernes får feil beskjed "bruker skrånende ' blir funnet" inne telefonkatalog, behage prøve atter der hvor utsendelsen type er bruker ikke inne adresseliste.</span><span class="sxs-lookup"><span data-stu-id="a9450-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="a9450-104">Følgende trinn kan fullføres for å feilsøke problemet.</span><span class="sxs-lookup"><span data-stu-id="a9450-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="a9450-105">Kontroller at kontoen som godtok invitasjonen til e-post, er den samme kontoen som brukes til å logge på senere.</span><span class="sxs-lookup"><span data-stu-id="a9450-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="a9450-106">Kontroller at brukeren bruker samme konto til å godta invitasjonen og logge på området.</span><span class="sxs-lookup"><span data-stu-id="a9450-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="a9450-107">Hvis du vil ha mer informasjon, kan du se Administrere [aliaser for</a> Microsoft-kontoen din for å administrere Office 365-påloggingen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="a9450-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="a9450-108">Bla til hvert område (r) der brukeren mottar feilen.</span><span class="sxs-lookup"><span data-stu-id="a9450-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="a9450-109">Legg til "/_layouts/15/People.aspx/membershipgroupid = 0" (i doble anførselstegn) til slutten av webadressen.</span><span class="sxs-lookup"><span data-stu-id="a9450-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="a9450-110">Eksempel: https://< "Contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="a9450-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="a9450-111">Velg brukeren fra listen.</span><span class="sxs-lookup"><span data-stu-id="a9450-111">Select the user from the list.</span></span>

- <span data-ttu-id="a9450-112">Klikk **Fjern brukertillatelser** fra båndet.</span><span class="sxs-lookup"><span data-stu-id="a9450-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="a9450-113">Legg til brukeren og Send invitasjonen til brukeren på nytt.</span><span class="sxs-lookup"><span data-stu-id="a9450-113">Add back the User and Resend the invite to the user.</span></span>

