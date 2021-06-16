---
title: Active Directory synkroniseres ikke
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930984"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="e3dde-102">Active Directory synkroniseres ikke</span><span class="sxs-lookup"><span data-stu-id="e3dde-102">Active Directory not syncing</span></span>

<span data-ttu-id="e3dde-103">Hvis du mottar synkroniseringsfeil, for eksempel «ingen nylig synkronisering», eller legger merke til katalogsynkroniseringsstatusen i Office-administrasjonsportalen, sier «Sist synkronisert for mer enn 3 dager siden», kan det være at AADConnect har feil innstillinger eller utilstrekkelige tillatelser til å utføre en synkronisering.</span><span class="sxs-lookup"><span data-stu-id="e3dde-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="e3dde-104">Hvis du installerer AADConnect på nytt ved hjelp av hurtiginnstillinger, kan problemet løses raskt:</span><span class="sxs-lookup"><span data-stu-id="e3dde-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="e3dde-105">[Last ned den nyeste versjonen av AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="e3dde-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="e3dde-106">[Følg instruksjonene for ekspressinstallasjon](/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="e3dde-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="e3dde-107">Azure AD Connect må installeres på Windows-2012 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="e3dde-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="e3dde-108">Denne serveren må være domene-tilkoblet og være en domenekontroller eller en medlemsserver.</span><span class="sxs-lookup"><span data-stu-id="e3dde-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="e3dde-109">Hvis du vil ha en fullstendig liste over Azure AD Koble til krav og forhåndskrav, kan du se gjennom Forutsetninger [for Azure AD Koble til.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="e3dde-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="e3dde-110">Hvis du vil ha mer informasjon om AADConnect-tjenestekontoer, [kan du se Azure AD Koble til: Kontoer og tillatelser](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="e3dde-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
