---
title: Gjenopprette en slettet fil eller mappe
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 604690e62f09b7ca0618c4a581605e22f19a7732
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507460"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="236e0-102">Gjenopprette en slettet fil eller mappe</span><span class="sxs-lookup"><span data-stu-id="236e0-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="236e0-103">SharePoint Online beholder sikkerhetskopier av alt innhold for 14 flere dager utover faktisk sletting.</span><span class="sxs-lookup"><span data-stu-id="236e0-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="236e0-104">Hvis innhold ikke kan gjenopprettes via papirkurven eller gjenopprette filer, kan en administrator kontakte Microsoft Support for å be om en gjenoppretting helst i 14 dag-vinduet.</span><span class="sxs-lookup"><span data-stu-id="236e0-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="236e0-105">Restorations fra sikkerhetskopier kan bare fullføres for områdesamlinger eller sekundære områder, ikke for bestemte filer, lister eller biblioteker.</span><span class="sxs-lookup"><span data-stu-id="236e0-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="236e0-106">Når du sletter et element eller et område fra Sharepoint, er ikke det umiddelbart fjernet.</span><span class="sxs-lookup"><span data-stu-id="236e0-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="236e0-107">Slettede elementer går inn i papirkurven for en bestemt tidsperiode.</span><span class="sxs-lookup"><span data-stu-id="236e0-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="236e0-108">Du kan gjenopprette elementer som du slettet til sin opprinnelige plassering i den perioden.</span><span class="sxs-lookup"><span data-stu-id="236e0-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="236e0-109">Hvis du vil ha mer informasjon, kan du besøke koblingene nedenfor.</span><span class="sxs-lookup"><span data-stu-id="236e0-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="236e0-110">[Gjenopprette elementer i papirkurven på SharePoint-området](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="236e0-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

[<span data-ttu-id="236e0-111">Gjenopprette slettede filer eller mapper i OneDrive</span><span class="sxs-lookup"><span data-stu-id="236e0-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="236e0-112">Gjenopprette en slettet områdesamling (inkludert grupper, kommunikasjon og andre områder)</span><span class="sxs-lookup"><span data-stu-id="236e0-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="236e0-113">Gjenopprette et slettet område for OneDrive</span><span class="sxs-lookup"><span data-stu-id="236e0-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="236e0-114">Administratorer kan vurdere å bruke [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)for bulk recycle bin handlinger.</span><span class="sxs-lookup"><span data-stu-id="236e0-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="236e0-115">**Funksjonen for gjenoppretting av filer**</span><span class="sxs-lookup"><span data-stu-id="236e0-115">**Files Restore feature**</span></span>

<span data-ttu-id="236e0-116">Hvis mange av filene dine OneDrive eller SharePoint få slettet, overskrives, skadet eller infisert av skadelig programvare, kan du gjenopprette hele OneDrive eller SharePoint-biblioteket til et tidligere tidspunkt ved hjelp av funksjonen for gjenoppretting av filer.</span><span class="sxs-lookup"><span data-stu-id="236e0-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="236e0-117">Gjenopprette et bibliotek for OneDrive</span><span class="sxs-lookup"><span data-stu-id="236e0-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="236e0-118">Gjenopprette et dokumentbibliotek</span><span class="sxs-lookup"><span data-stu-id="236e0-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a?ui=en-US&amp;rs=en-US&amp;ad=US.)

