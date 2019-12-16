---
title: Feilsøking av tilgang nektet meldinger til OneDrive for Business-områder
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9d8aba4e53a1e0505a430296bb1c11713ea2ce7b
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051614"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="019cc-102">Feilsøking av tilgang nektet meldinger til OneDrive for Business-områder</span><span class="sxs-lookup"><span data-stu-id="019cc-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="019cc-103">Dette problemet oppstår hyppigst når en bruker slettes og opprettes på nytt med samme hovednavn for bruker (UPN).</span><span class="sxs-lookup"><span data-stu-id="019cc-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="019cc-104">Den nye kontoen opprettes ved hjelp av en annen verdi for PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="019cc-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="019cc-105">Når brukeren prøver å få tilgang til en områdesamling eller deres OneDrive, har brukeren en feil PUID.</span><span class="sxs-lookup"><span data-stu-id="019cc-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="019cc-106">Et annet scenario omfatter katalogsynkronisering med en organisasjonsenhet for Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="019cc-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="019cc-107">Hvis brukere allerede har logget på SharePoint, og deretter flyttes til en annen ORGANISASJONSENHET og resynced med SharePoint, kan de oppleve dette problemet.</span><span class="sxs-lookup"><span data-stu-id="019cc-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="019cc-108">Hvis du vil løse dette problemet, bør du gjenopprette den opprinnelige UPN med trinnene i artikkelen, [gjenopprette en bruker i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="019cc-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="019cc-109">Hvis du ikke kan gjenopprette den opprinnelige brukeren, bør du fjerne den gamle brukeren fra OneDrive-området ved hjelp av disse trinnene, [fjerne en bruker fra listen over bruker informasjon]().</span><span class="sxs-lookup"><span data-stu-id="019cc-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="019cc-110">Når dette er gjort, kan du kontrollere at brukeren har admin rettigheter til OneDrive-området ved å følge fremgangsmåten for å [legge til admin for en brukers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="019cc-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="019cc-111">Hvis du vil ha mer informasjon om tillatelsesnivåer, kan du se artikkelen [forstå tillatelsesnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="019cc-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
