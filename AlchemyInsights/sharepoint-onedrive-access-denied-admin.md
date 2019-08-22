---
title: Feilsøking i forbindelse med tilgang til meldinger
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 0a885e15d54c9337711f2528628789dfcb903264
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36503542"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="78d4d-102">Feilsøking i forbindelse med tilgang meldinger i administrasjonssenteret for Sharepoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="78d4d-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="78d4d-103">Hvis du mottar meldingen Ingen tilgang når du forsøker å gå til administrasjonssenteret en Sharepoint/OneDrive, må du kontrollere at du [tilordner en lisens for brukeren](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="78d4d-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="78d4d-104">Hvis brukeren har en lisens, bør du også kontrollere at de er [tilordnet en administrator-rolle](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) som har tilgang til admin-sentre.</span><span class="sxs-lookup"><span data-stu-id="78d4d-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="78d4d-105">Dette problemet kan også oppstå når en bruker slettes og opprettes på nytt med samme brukerhovednavnet (UPN).</span><span class="sxs-lookup"><span data-stu-id="78d4d-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="78d4d-106">Den nye kontoen er opprettet ved hjelp av en annen verdi for PUID (unik ID for Passport).</span><span class="sxs-lookup"><span data-stu-id="78d4d-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="78d4d-107">Når brukeren prøver å få tilgang til en områdesamling eller sin OneDrive, har brukeren en feil PUID.</span><span class="sxs-lookup"><span data-stu-id="78d4d-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="78d4d-108">Andre scenariet omfatter directory-synkronisering med en Active Directory-organisasjonsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="78d4d-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="78d4d-109">Hvis brukere har allerede logget på SharePoint, er flyttet til en annen Organisasjonsenhet og resynced med SharePoint, kan de oppleve dette problemet.</span><span class="sxs-lookup"><span data-stu-id="78d4d-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="78d4d-110">Hvis du vil løse dette problemet, bør du gjenopprette den opprinnelige UPN med trinnene i artikkelen, [gjenopprette en brukers i Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="78d4d-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="78d4d-111">Merk: Hvis en OneDrive eller en SharePoint-administrator center ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være en midlertidig tjeneste problem.</span><span class="sxs-lookup"><span data-stu-id="78d4d-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="78d4d-112">[Kontroller service helse instrumentbordet](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="78d4d-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


