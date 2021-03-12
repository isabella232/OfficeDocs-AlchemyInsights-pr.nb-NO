---
title: Feilsøk meldinger om ingen tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707963"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="362c7-102">Feilsøke meldinger ingen tilgang i administrasjonssenteret for SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="362c7-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="362c7-103">Hvis du får melding om at tilgangen er avvist når du prøver å gå til administrasjonssenteret for Sharepoint/OneDrive, må du kontrollere at du tilordner en lisens [til brukeren.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="362c7-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="362c7-104">Hvis brukeren har en lisens, bør du også kontrollere at de er tilordnet en [administratorrolle](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) som har tilgang til administrasjonssentrene.</span><span class="sxs-lookup"><span data-stu-id="362c7-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="362c7-105">Dette problemet kan også oppstå når en bruker slettes og opprettes på nytt med samme brukerprinsippnavn (UPN).</span><span class="sxs-lookup"><span data-stu-id="362c7-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="362c7-106">Den nye kontoen opprettes ved hjelp av en annen PUID-verdi (Pass unik ID).</span><span class="sxs-lookup"><span data-stu-id="362c7-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="362c7-107">Når brukeren prøver å få tilgang til en områdesamling eller oneDrive, har brukeren feil PUID.</span><span class="sxs-lookup"><span data-stu-id="362c7-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="362c7-108">En annen situasjon innebærer katalogsynkronisering med en Active Directory-organisasjonsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="362c7-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="362c7-109">Hvis brukere allerede har logget på SharePoint, og deretter flyttes til en annen organisasjonsadministrasjon og synkroniseres med SharePoint på nytt, kan de oppleve dette problemet.</span><span class="sxs-lookup"><span data-stu-id="362c7-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="362c7-110">Du kan løse dette problemet ved å gjenopprette det opprinnelige UPN-navnet ved hjelp av fremgangsmåten i artikkelen Gjenopprette en [bruker i Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)</span><span class="sxs-lookup"><span data-stu-id="362c7-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="362c7-111">Obs! Hvis et administrasjonssenter for OneDrive eller SharePoint ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et midlertidig tjenesteproblem.</span><span class="sxs-lookup"><span data-stu-id="362c7-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="362c7-112">[Kontroller tilstandsinstrumentbordet](https://portal.office.com/adminportal/home#/servicehealth)for tjenesten.</span><span class="sxs-lookup"><span data-stu-id="362c7-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


