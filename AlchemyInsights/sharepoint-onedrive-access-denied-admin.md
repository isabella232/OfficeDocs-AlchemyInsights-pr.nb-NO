---
title: Feilsøking i forbindelse med nektet tilgang
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751285"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="71437-102">Feilsøking i forbindelse med tilgang nektet meldinger i administrasjonssenteret for SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="71437-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="71437-103">Hvis du får meldingen ingen tilgang når du prøver å bla til et Administrasjonssenter for SharePoint/OneDrive, må du kontrollere at du [tilordner en lisens til brukeren](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="71437-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="71437-104">Hvis brukeren har en lisens, bør du også kontrollere at de er [tilordnet en administratorrolle](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) som kan få tilgang til administrasjons sentrene.</span><span class="sxs-lookup"><span data-stu-id="71437-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="71437-105">Dette problemet kan også oppstå når en bruker er slettet og opprettet på nytt med samme hovednavn for bruker (UPN).</span><span class="sxs-lookup"><span data-stu-id="71437-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="71437-106">Den nye kontoen opprettes ved hjelp av en annen verdi for PUID (Passport Unique ID).</span><span class="sxs-lookup"><span data-stu-id="71437-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="71437-107">Når brukeren prøver å få tilgang til en områdesamling eller deres OneDrive, har brukeren en feil PUID.</span><span class="sxs-lookup"><span data-stu-id="71437-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="71437-108">Et annet scenario omfatter katalogsynkronisering med en organisasjonsenhet for Active Directory (OU).</span><span class="sxs-lookup"><span data-stu-id="71437-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="71437-109">Hvis brukere allerede har logget på SharePoint, og deretter flyttes til en annen ORGANISASJONSENHET og resynced med SharePoint, kan de oppleve dette problemet.</span><span class="sxs-lookup"><span data-stu-id="71437-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="71437-110">Hvis du vil løse dette problemet, bør du gjenopprette den opprinnelige UPN med trinnene i artikkelen, [gjenopprette en bruker i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="71437-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="71437-111">Merk: Hvis et OneDrive eller Administrasjonssenter for SharePoint ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et midlertidig problem med tjenesten.</span><span class="sxs-lookup"><span data-stu-id="71437-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="71437-112">[Kontroller instrumentbordet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="71437-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


