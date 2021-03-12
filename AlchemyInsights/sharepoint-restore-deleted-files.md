---
title: Gjenopprette en slettet fil eller mappe
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 8c7ce48f50b5c933ea15c23a486b99ad7a7f4d79
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707531"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="2128c-102">Gjenopprette en slettet fil eller mappe</span><span class="sxs-lookup"><span data-stu-id="2128c-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="2128c-103">SharePoint Online beholder sikkerhetskopier av alt innhold i 14 ekstra dager etter faktisk sletting.</span><span class="sxs-lookup"><span data-stu-id="2128c-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="2128c-104">Hvis innholdet ikke kan gjenopprettes via papirkurven eller Filgjenoppretting, kan en administrator kontakte Microsoft Kundestøtte for å be om gjenoppretting når som helst i vinduet på 14 dager.</span><span class="sxs-lookup"><span data-stu-id="2128c-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="2128c-105">Gjenoppretting fra sikkerhetskopier kan bare fullføres for områdesamlinger eller sekundære områder, ikke for spesifikke filer, lister eller biblioteker.</span><span class="sxs-lookup"><span data-stu-id="2128c-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="2128c-106">Når du sletter et element eller et nettsted fra SharePoint, fjernes det ikke umiddelbart.</span><span class="sxs-lookup"><span data-stu-id="2128c-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="2128c-107">Slettede elementer sendes til papirkurven i en tidsperiode.</span><span class="sxs-lookup"><span data-stu-id="2128c-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="2128c-108">I løpet av den perioden kan du gjenopprette elementene du slettet, til de opprinnelige plasseringene.</span><span class="sxs-lookup"><span data-stu-id="2128c-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="2128c-109">Hvis du vil ha mer informasjon, kan du ta en titt på koblingen under.</span><span class="sxs-lookup"><span data-stu-id="2128c-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="2128c-110">[Gjenopprette elementer i papirkurven på et SharePoint-område.](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be)</span><span class="sxs-lookup"><span data-stu-id="2128c-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span></span>

[<span data-ttu-id="2128c-111">Gjenopprette slettede filer eller mapper i OneDrive</span><span class="sxs-lookup"><span data-stu-id="2128c-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="2128c-112">Gjenopprette en slettet områdesamling (inkludert gruppe, kommunikasjon og andre områder)</span><span class="sxs-lookup"><span data-stu-id="2128c-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="2128c-113">Gjenopprette et slettet OneDrive-område</span><span class="sxs-lookup"><span data-stu-id="2128c-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="2128c-114">Administratorer kan vurdere å bruke [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)for masseutgavehandlinger for papirkurven.</span><span class="sxs-lookup"><span data-stu-id="2128c-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="2128c-115">**Gjenopprett filer-funksjon**</span><span class="sxs-lookup"><span data-stu-id="2128c-115">**Files Restore feature**</span></span>

<span data-ttu-id="2128c-116">Hvis mange av OneDrive- eller SharePoint-filene slettes, overskrives, skades eller infiserer av skadelig programvare, kan du gjenopprette hele OneDrive- eller SharePoint-biblioteket til et tidligere tidspunkt ved hjelp av filgjenopprettingsfunksjonen.</span><span class="sxs-lookup"><span data-stu-id="2128c-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="2128c-117">Gjenopprette et OneDrive-bibliotek</span><span class="sxs-lookup"><span data-stu-id="2128c-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="2128c-118">Gjenopprette et dokumentbibliotek</span><span class="sxs-lookup"><span data-stu-id="2128c-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

