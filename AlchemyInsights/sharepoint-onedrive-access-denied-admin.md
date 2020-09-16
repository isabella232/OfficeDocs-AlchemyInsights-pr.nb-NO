---
title: Feilsøke meldinger om ingen tilgang
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767671"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="ff829-102">Feilsøke tilgang til meldinger som nektes i administrasjons senteret for SharePoint/OneDrive</span><span class="sxs-lookup"><span data-stu-id="ff829-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="ff829-103">Hvis du mottar en melding om at du ikke får tilgang når du prøver å bla til et administrasjons senter for SharePoint/OneDrive, må du sørge for at du [tilordner en lisens til brukeren](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="ff829-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="ff829-104">Hvis brukeren har en lisens, bør du også sørge for at de er [tilordnet en administrator rolle](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) som har tilgang til administrasjons sentrene.</span><span class="sxs-lookup"><span data-stu-id="ff829-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="ff829-105">Dette problemet kan også oppstå når en bruker slettes og opprettes på nytt med samme brukerhovednavn (UPN).</span><span class="sxs-lookup"><span data-stu-id="ff829-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="ff829-106">Den nye kontoen opprettes ved hjelp av en annen PUID-verdi (konto – unik ID).</span><span class="sxs-lookup"><span data-stu-id="ff829-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="ff829-107">Når brukeren prøver å få tilgang til en område samling eller deres OneDrive, har brukeren feil PUID.</span><span class="sxs-lookup"><span data-stu-id="ff829-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="ff829-108">Et annet scenario omfatter katalog synkronisering med en Active Directory-organisasjonsenhet (OU).</span><span class="sxs-lookup"><span data-stu-id="ff829-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="ff829-109">Hvis brukerne allerede har logget seg på SharePoint, og deretter flyttes til en annen OU og synkroniseres med SharePoint, kan de oppleve dette problemet.</span><span class="sxs-lookup"><span data-stu-id="ff829-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="ff829-110">Du kan løse dette problemet ved å gjenopprette den opprinnelige UPN-en med trinnene i artikkelen, [gjenopprette en bruker i Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="ff829-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="ff829-111">Obs! hvis et administrasjons senter for OneDrive eller SharePoint ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et midlertidig tjeneste problem.</span><span class="sxs-lookup"><span data-stu-id="ff829-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="ff829-112">[Kontroller instrument bordet for tjeneste tilstand](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="ff829-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


