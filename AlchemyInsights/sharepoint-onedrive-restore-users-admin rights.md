---
title: Feilsøke tilgang nektet meldinger til OneDrive for Business-områder
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670625"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="59824-102">Feilsøke tilgang nektet meldinger til OneDrive for Business-områder</span><span class="sxs-lookup"><span data-stu-id="59824-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="59824-103">Dette problemet oppstår oftest når en bruker slettes og opprettes på nytt med samme brukerhovednavn (UPN).</span><span class="sxs-lookup"><span data-stu-id="59824-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="59824-104">Den nye kontoen opprettes ved hjelp av en annen PUID-verdi (konto – unik ID).</span><span class="sxs-lookup"><span data-stu-id="59824-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="59824-105">Når brukeren prøver å få tilgang til en område samling eller deres OneDrive, har brukeren feil PUID.</span><span class="sxs-lookup"><span data-stu-id="59824-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="59824-106">Et annet scenario omfatter katalog synkronisering med en Active Directory-organisasjonsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="59824-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="59824-107">Hvis brukerne allerede har logget seg på SharePoint, og deretter flyttes til en annen OU og synkroniseres med SharePoint, kan de oppleve dette problemet.</span><span class="sxs-lookup"><span data-stu-id="59824-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="59824-108">Hvis du vil løse dette problemet, må du gjenopprette den opprinnelige UPN-en med trinnene i artikkelen, [gjenopprette en bruker i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="59824-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="59824-109">Hvis du ikke kan gjenopprette den opprinnelige brukeren, må du fjerne den gamle brukeren fra OneDrive-nettstedet ved hjelp av disse trinnene, [fjerne en bruker fra bruker informasjons listen]().</span><span class="sxs-lookup"><span data-stu-id="59824-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="59824-110">Når dette er gjort, kan du kontrollere at brukeren har administrator rettigheter til OneDrive-nettstedet ved å følge Fremgangs måten [for å legge til administrator for en brukers OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="59824-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="59824-111">Hvis du vil ha mer informasjon om tillatelses nivåer, kan du se artikkelen [forstå tilgangs nivåer i SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="59824-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
