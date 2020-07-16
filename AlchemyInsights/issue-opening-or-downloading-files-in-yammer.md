---
title: Utstede åpning eller nedlasting av filer i Yammer
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
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148335"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="4b54f-102">Utstede åpning eller nedlasting av filer i Yammer</span><span class="sxs-lookup"><span data-stu-id="4b54f-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="4b54f-103">Classic Yammer støtter flere alternativer for filopplastinger til meldinger og grupper.</span><span class="sxs-lookup"><span data-stu-id="4b54f-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="4b54f-104">Avhengig av nettverkskonfigurasjon, filer som er standard til lagring i SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4b54f-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="4b54f-105">Filvelgeren i nye Yammer støtter ennå ikke alle alternativene som er tilgjengelige i klassisk Yammer.</span><span class="sxs-lookup"><span data-stu-id="4b54f-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="4b54f-106">En fremtidig oppdatering vil legge til flere funksjoner.</span><span class="sxs-lookup"><span data-stu-id="4b54f-106">A future update will add additional features.</span></span> <span data-ttu-id="4b54f-107">Hvis du vil ha mer informasjon, kan du se [Legge ved en fil eller et bilde i et Yammer-samtaleinnlegg](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="4b54f-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="4b54f-108">**Kan ikke åpne eller laste ned en fil**</span><span class="sxs-lookup"><span data-stu-id="4b54f-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="4b54f-109">En fil kan laste opp til Yammer, men også koble til en fil i SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="4b54f-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="4b54f-110">Hvis du vil feilsøke, må du først bestemme plasseringen av filen.</span><span class="sxs-lookup"><span data-stu-id="4b54f-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="4b54f-111">Hvis filen er lastet opp til Yammer, vil den ha en \*.yammer.com URL-adresse.</span><span class="sxs-lookup"><span data-stu-id="4b54f-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="4b54f-112">Kontroller at nødvendige URL-adresser og IP-adresser er blokkert.</span><span class="sxs-lookup"><span data-stu-id="4b54f-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="4b54f-113">Hvis du vil ha mer informasjon, kan du se blogginnlegget [Ved hjelp av hardkodede IP-adresser for Yammer anbefales ikke](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="4b54f-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="4b54f-114">Kontroller om en bruker som også er en global administrator, kan laste ned filen.</span><span class="sxs-lookup"><span data-stu-id="4b54f-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="4b54f-115">Hvis filen er privat, må du kanskje bruke modus for privat innhold.</span><span class="sxs-lookup"><span data-stu-id="4b54f-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="4b54f-116">Hvis du vil ha mer informasjon, kan du se [Overvåke privat innhold i Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="4b54f-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="4b54f-117">**Yammer-gjester og -filer på nettverksnivå i SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="4b54f-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="4b54f-118">[Gjester på nettverksnivå i Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) bruker ikke Azure AD B2B og er interne for Yammer-tjenesten, slik at de ikke får tilgang til Yammer-filer som er lagret i SharePoint.</span><span class="sxs-lookup"><span data-stu-id="4b54f-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="4b54f-119">Opprett en ekstern AAD B2B-bruker som har tilgang til dokumentbiblioteker i SharePoint Online ved hjelp av denne identiteten.</span><span class="sxs-lookup"><span data-stu-id="4b54f-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="4b54f-120">Hvis du vil ha informasjon om fremtidig kundestøtte for Azure AD B2B-gjester i Yammer, kan du se [Kundestøtte for Business-to-business (B2B) i Yammer Preview – Kundevilkår og vanlige spørsmål](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="4b54f-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>