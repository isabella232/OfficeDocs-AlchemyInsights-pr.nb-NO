---
title: Feilsøke problemer med innlasting av bilder i Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148293"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="e6c6e-102">Feilsøke problemer med innlasting av bilder i Yammer</span><span class="sxs-lookup"><span data-stu-id="e6c6e-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="e6c6e-103">Når det oppstår problemer med bilder og forhåndsvisninger av filer i Yammer, kan du feilsøke ved å kontrollere om problemet oppstår for alle brukere, om det skjer på mobile enheter, og hvis det er reproduserbart når du laster opp vedlegget.</span><span class="sxs-lookup"><span data-stu-id="e6c6e-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="e6c6e-104">**Problemer med profilbilde**</span><span class="sxs-lookup"><span data-stu-id="e6c6e-104">**Profile photo issues**</span></span>  

<span data-ttu-id="e6c6e-105">Hvis sluttbrukere logger på Yammer via Microsoft 365, må de endre profilen, inkludert profilbildet.</span><span class="sxs-lookup"><span data-stu-id="e6c6e-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="e6c6e-106">Hvis brukere ikke har tillatelse til å gjøre profiloppdateringer, kan en administrator gjøre oppdateringen for brukeren.</span><span class="sxs-lookup"><span data-stu-id="e6c6e-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="e6c6e-107">Hvis du vil ha mer informasjon, kan du se [Vise og oppdatere profilen i Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="e6c6e-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="e6c6e-108">Hvis du vil ha informasjon om profilredigering, inkludert profilbilder, kan du se [Endre Yammer-profilen og -innstillingene](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="e6c6e-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="e6c6e-109">Oppdaterte profilbilder synkroniseres på en annen måte enn profilattributter.</span><span class="sxs-lookup"><span data-stu-id="e6c6e-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="e6c6e-110">Brukere må logge på for å starte en synkronisering av profilbildet sitt.</span><span class="sxs-lookup"><span data-stu-id="e6c6e-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="e6c6e-111">Hvis du vil ha mer informasjon, kan du se [brukerprofilbilder som er oppdatert fra Office 365 til Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="e6c6e-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="e6c6e-112">Hvis du vil ha informasjon om brukerlivssyklusen for Yammer, kan du se [Administrere Yammer-brukere på tvers av livssyklusen fra Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="e6c6e-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="e6c6e-113">Hvis du vil ha mer informasjon om hvordan profilbildesynkronisering fungerer i Microsoft 365, kan du se [Informasjon om profilbildesynkronisering i Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="e6c6e-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="e6c6e-114">**Forhåndsvisninger av dokumenter og miniatyrproblemer for bilder**</span><span class="sxs-lookup"><span data-stu-id="e6c6e-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="e6c6e-115">Når filer eller bilder legges ut i Yammer, vises kanskje ikke forhåndsvisninger fordi:</span><span class="sxs-lookup"><span data-stu-id="e6c6e-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="e6c6e-116">Filen er skadet og kan ikke behandles.</span><span class="sxs-lookup"><span data-stu-id="e6c6e-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="e6c6e-117">Filen er ikke nylig lastet opp til SharePoint Online, eller Yammer har ugyldige metadata av andre grunner.</span><span class="sxs-lookup"><span data-stu-id="e6c6e-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="e6c6e-118">URL-adresser som kreves for lasting av forhåndsvisningsbildene, blokkeres.</span><span class="sxs-lookup"><span data-stu-id="e6c6e-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="e6c6e-119">Forhåndsvisningen av filen ble fjernet av brukeren før postering.</span><span class="sxs-lookup"><span data-stu-id="e6c6e-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="e6c6e-120">Et tjenesteproblem forhindret at en forhåndsvisning ble generert.</span><span class="sxs-lookup"><span data-stu-id="e6c6e-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="e6c6e-121">**Merk at** Forhåndsvisninger for koblinger og filopplastinger kan oppføre seg annerledes.</span><span class="sxs-lookup"><span data-stu-id="e6c6e-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="e6c6e-122">Koblinger til filer på Internett eller koblinger som krever ekstra godkjenning, vises kanskje ikke riktig.</span><span class="sxs-lookup"><span data-stu-id="e6c6e-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="e6c6e-123">Hvis du vil ha mer informasjon, kan du se [Legge ved en fil eller et bilde i en Yammer-melding](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="e6c6e-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 