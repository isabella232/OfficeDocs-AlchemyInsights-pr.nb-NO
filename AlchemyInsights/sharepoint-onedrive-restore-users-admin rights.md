---
title: Feilsøke access-avslåtte meldinger til OneDrive for Business-områder
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511193"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="e1272-102">Feilsøke access-avslåtte meldinger til OneDrive for Business-områder</span><span class="sxs-lookup"><span data-stu-id="e1272-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="e1272-103">Dette problemet oppstår oftest når en bruker slettes og opprettes på nytt med samme brukerhovednavn (UPN).</span><span class="sxs-lookup"><span data-stu-id="e1272-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="e1272-104">Den nye kontoen opprettes ved hjelp av en annen PUID-verdi (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="e1272-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="e1272-105">Når brukeren prøver å få tilgang til en områdesamling eller OneDrive, har brukeren en feil PUID.</span><span class="sxs-lookup"><span data-stu-id="e1272-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="e1272-106">Et annet scenario innebærer katalogsynkronisering med en Active Directory-organisasjonsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="e1272-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="e1272-107">Hvis brukere allerede har logget på SharePoint, og deretter flyttes til en annen organisasjon og synkroniseres på nytt med SharePoint, kan det oppstå dette problemet.</span><span class="sxs-lookup"><span data-stu-id="e1272-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="e1272-108">Hvis du vil løse dette problemet, bør du gjenopprette det opprinnelige UPN med trinnene i artikkelen, [Gjenopprette en bruker i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="e1272-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="e1272-109">Hvis du ikke kan gjenopprette den opprinnelige brukeren, bør du fjerne den gamle brukeren fra OneDrive-området ved hjelp av disse trinnene, [fjerne en bruker fra brukerinformasjonslisten]().</span><span class="sxs-lookup"><span data-stu-id="e1272-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="e1272-110">Når dette er gjort, kan du kontrollere at brukeren har administratorrettigheter til OneDrive-området ved å følge trinnene [for å legge til administratorer for en brukers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="e1272-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="e1272-111">Hvis du vil ha mer informasjon om tillatelsesnivåer, kan du se artikkelen [Forstå tillatelsesnivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="e1272-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
