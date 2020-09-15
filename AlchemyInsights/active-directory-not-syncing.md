---
title: Active Directory ikke synkronisere
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697638"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="e8e74-102">Active Directory ikke synkronisere</span><span class="sxs-lookup"><span data-stu-id="e8e74-102">Active Directory not syncing</span></span>

<span data-ttu-id="e8e74-103">Hvis du får synkroniserings feil, for eksempel «ingen nylig synkronisering», eller Legg merke til at statusen for katalog synkronisering i Office Admin-portalen sier at «sist synkronisert for mer enn 3 dager siden», kan være at AADConnect har feil innstillinger eller utilstrekkelige tillatelser til å utføre en synkronisering.</span><span class="sxs-lookup"><span data-stu-id="e8e74-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="e8e74-104">Å installere AADConnect på nytt ved hjelp av innstillingene for Express kan løse problemet raskt:</span><span class="sxs-lookup"><span data-stu-id="e8e74-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="e8e74-105">[Last ned den nyeste versjonen av AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="e8e74-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="e8e74-106">[Følg instruksjonene for hurtig installasjon](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="e8e74-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="e8e74-107">Hvis du vil ha mer informasjon om AADConnect-tjeneste kontoer, kan du se [Azure ad Connect: kontoer og tillatelser](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="e8e74-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
