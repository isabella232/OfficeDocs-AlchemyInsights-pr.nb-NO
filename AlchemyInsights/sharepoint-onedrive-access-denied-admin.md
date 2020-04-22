---
title: Feilsøke ingen meldinger om tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758483"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="eecd9-102">Feilsøke ingen tilgang i administrasjonssenteret for Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="eecd9-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="eecd9-103">Hvis du mottar en melding om ingen tilgang når du prøver å bla til et administrasjonssenter for Sharepoint/OneDrive, må du kontrollere at du [tilordner en lisens til brukeren](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="eecd9-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="eecd9-104">Hvis brukeren har en lisens, bør du også kontrollere at de er [tilordnet en administratorrolle](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) som har tilgang til administrasjonssentrene.</span><span class="sxs-lookup"><span data-stu-id="eecd9-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="eecd9-105">Dette problemet kan også oppstå når en bruker slettes og opprettes på nytt med samme brukerhovednavn (UPN).</span><span class="sxs-lookup"><span data-stu-id="eecd9-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="eecd9-106">Den nye kontoen opprettes ved hjelp av en annen PUID-verdi (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="eecd9-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="eecd9-107">Når brukeren prøver å få tilgang til en områdesamling eller OneDrive, har brukeren en feil PUID.</span><span class="sxs-lookup"><span data-stu-id="eecd9-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="eecd9-108">Et annet scenario innebærer katalogsynkronisering med en Active Directory-organisasjonsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="eecd9-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="eecd9-109">Hvis brukere allerede har logget på SharePoint, og deretter flyttes til en annen ORGANISASJON og synkroniseres på nytt med SharePoint, kan de oppleve dette problemet.</span><span class="sxs-lookup"><span data-stu-id="eecd9-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="eecd9-110">Hvis du vil løse dette problemet, bør du gjenopprette den opprinnelige UPN med trinnene i artikkelen, [Gjenopprette en bruker i Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="eecd9-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="eecd9-111">Merk: Hvis et administrasjonssenter for OneDrive eller SharePoint ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et midlertidig tjenesteproblem.</span><span class="sxs-lookup"><span data-stu-id="eecd9-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="eecd9-112">[Kontroller instrumentbordet for servicetilstand](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="eecd9-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


