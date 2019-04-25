---
title: 932 oppgraderer AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8ffa8f64019077034bc4fad61d1d843849c42898
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32389726"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="ac98c-102">Oppgradering Azure AD koble</span><span class="sxs-lookup"><span data-stu-id="ac98c-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="ac98c-103">Som standard aktiveres automatisk oppgradering for Azure AD-tilkobling, som bidrar til å sikre at du kjører den nyeste versjonen.</span><span class="sxs-lookup"><span data-stu-id="ac98c-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="ac98c-104">Hvis du vil kontrollere innstillingene for automatisk oppgradering, kan du bruke cmdleten **Get-ADSyncAutoUpgrade** i Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ac98c-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="ac98c-105">Cmdleten vil returnere en av følgende verdier:</span><span class="sxs-lookup"><span data-stu-id="ac98c-105">The cmdlet will return one of following values:</span></span> 

- <span data-ttu-id="ac98c-106">**Aktivert**: automatisk oppgradering er aktivert.</span><span class="sxs-lookup"><span data-stu-id="ac98c-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="ac98c-107">**Deaktivert**: automatisk oppgradering er deaktivert.</span><span class="sxs-lookup"><span data-stu-id="ac98c-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="ac98c-108">**Suspended**: systemet er ikke lenger berettiget til å motta automatiske oppgraderinger.</span><span class="sxs-lookup"><span data-stu-id="ac98c-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="ac98c-109">Du kan ikke konfigurere denne verdien. Det er satt av systemet.</span><span class="sxs-lookup"><span data-stu-id="ac98c-109">You can't configure this value; it's set by the system.</span></span> 

<span data-ttu-id="ac98c-110">Hvis du vil ha mer informasjon, kan du se [automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="ac98c-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="ac98c-111">Hvis du vil laste ned den nyeste versjonen av Azure AD-tilkobling, kan du gå til [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="ac98c-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
