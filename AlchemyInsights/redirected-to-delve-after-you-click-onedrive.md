---
title: OneDrive for Business Web OneDrive omdirigeres til Delve
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776388"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="61102-102">Omdirigert til Delve når du klikker OneDrive</span><span class="sxs-lookup"><span data-stu-id="61102-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="61102-103">Se vår detaljerte [veiledning for feil søking](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="61102-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="61102-104">Hvis du vil løse dette problemet, må administratoren gi brukerne rett til å opprette området mitt område.</span><span class="sxs-lookup"><span data-stu-id="61102-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="61102-105">Dette er fordi OneDrive for Business-siden er opprettet på mine områder.</span><span class="sxs-lookup"><span data-stu-id="61102-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="61102-106">Følg denne Fremgangs måten for å gi denne rettigheten:</span><span class="sxs-lookup"><span data-stu-id="61102-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="61102-107">Klikk **bruker profiler**i administrasjons senteret for SharePoint.</span><span class="sxs-lookup"><span data-stu-id="61102-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="61102-108">Klikk **Behandle bruker tillatelser**i **personer** -delen.</span><span class="sxs-lookup"><span data-stu-id="61102-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="61102-109">Legg til brukere som krever tillatelse for å opprette området mitt område.</span><span class="sxs-lookup"><span data-stu-id="61102-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="61102-110">Denne innstillingen er som standard satt til **alle unntatt eksterne brukere**.</span><span class="sxs-lookup"><span data-stu-id="61102-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="61102-111">Når du har lagt til brukeren, brukerne eller gruppen, må du kontrollere at brukeren som er lagt til, brukere eller grupper er valgt, bla til **tillatelser** -delen, og merk deretter av for **Opprett personlig område (obligatorisk for personlig lagring, nyhetsfeed og fulgt innhold)**.</span><span class="sxs-lookup"><span data-stu-id="61102-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="61102-112">Klikk **OK**, og la brukeren gå til OneDrive-siden for å opprette området.</span><span class="sxs-lookup"><span data-stu-id="61102-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
