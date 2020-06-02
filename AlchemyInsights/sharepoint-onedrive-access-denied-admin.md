---
title: Feilsøke access avviste meldinger
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505388"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="5c28e-102">Feilsøke access avviste meldinger i administrasjonssenteret for Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="5c28e-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="5c28e-103">Hvis du mottar en melding om tilgang når du prøver å gå til et administrasjonssenter for Sharepoint/OneDrive, må du kontrollere at du [tilordner en lisens til brukeren](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="5c28e-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="5c28e-104">Hvis brukeren har en lisens, bør du også kontrollere at de er [tilordnet en administratorrolle](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) som har tilgang til administrasjonssentrene.</span><span class="sxs-lookup"><span data-stu-id="5c28e-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="5c28e-105">Dette problemet kan også oppstå når en bruker slettes og opprettes på nytt med samme brukerhovednavn (UPN).</span><span class="sxs-lookup"><span data-stu-id="5c28e-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="5c28e-106">Den nye kontoen opprettes ved hjelp av en annen PUID-verdi (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="5c28e-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="5c28e-107">Når brukeren prøver å få tilgang til en områdesamling eller OneDrive, har brukeren en feil PUID.</span><span class="sxs-lookup"><span data-stu-id="5c28e-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="5c28e-108">Et annet scenario innebærer katalogsynkronisering med en Active Directory-organisasjonsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="5c28e-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="5c28e-109">Hvis brukere allerede har logget på SharePoint, og deretter flyttes til en annen organisasjon og synkroniseres på nytt med SharePoint, kan det oppstå dette problemet.</span><span class="sxs-lookup"><span data-stu-id="5c28e-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="5c28e-110">Hvis du vil løse dette problemet, bør du gjenopprette den opprinnelige UPN med trinnene i [artikkelen, Gjenopprette en bruker i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="5c28e-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="5c28e-111">Merk: Hvis et administrasjonssenter for OneDrive eller SharePoint ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et midlertidig tjenesteproblem.</span><span class="sxs-lookup"><span data-stu-id="5c28e-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="5c28e-112">[Kontroller instrumentbordet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="5c28e-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


