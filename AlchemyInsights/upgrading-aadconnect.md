---
title: 932 oppgradere AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806048"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="4b6c3-102">Oppgradere Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="4b6c3-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="4b6c3-103">Som standard er automatisk oppgradering aktivert for Azure AD Connect, noe som bidrar til å sikre at du kjører den nyeste versjonen.</span><span class="sxs-lookup"><span data-stu-id="4b6c3-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="4b6c3-104">Hvis du vil kontrollere innstillingene for automatisk oppgradering, kan du bruke **Get-ADSyncAutoUpgrade** -cmdleten i Azure ad PowerShell.</span><span class="sxs-lookup"><span data-stu-id="4b6c3-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="4b6c3-105">Cmdleten returnerer én av følgende verdier:</span><span class="sxs-lookup"><span data-stu-id="4b6c3-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="4b6c3-106">**Aktivert**: automatisk oppgradering er aktivert.</span><span class="sxs-lookup"><span data-stu-id="4b6c3-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="4b6c3-107">**Deaktivert**: automatisk oppgradering er deaktivert.</span><span class="sxs-lookup"><span data-stu-id="4b6c3-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="4b6c3-108">**Suspendert**: systemet er ikke lenger berettiget til å motta automatiske oppgraderinger.</span><span class="sxs-lookup"><span data-stu-id="4b6c3-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="4b6c3-109">Du kan ikke konfigurere denne verdien. den er angitt av systemet.</span><span class="sxs-lookup"><span data-stu-id="4b6c3-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="4b6c3-110">Hvis du vil ha mer informasjon, kan du se [automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="4b6c3-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="4b6c3-111">Hvis du vil laste ned den nyeste versjonen av Azure AD Connect, kan du gå til [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="4b6c3-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
