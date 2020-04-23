---
title: 932 Oppgradere AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766502"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="2192d-102">Oppgrader Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="2192d-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="2192d-103">Som standard er automatisk oppgradering aktivert for Azure AD Connect, noe som bidrar til å sikre at du kjører den nyeste versjonen.</span><span class="sxs-lookup"><span data-stu-id="2192d-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="2192d-104">Hvis du vil kontrollere de automatiske oppgraderingsinnstillingene, bruker du cmdleten **Get-ADSyncAutoUpgrade** i Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2192d-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="2192d-105">Cmdleten returnerer én av følgende verdier:</span><span class="sxs-lookup"><span data-stu-id="2192d-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="2192d-106">**Aktivert:** Automatisk oppgradering er aktivert.</span><span class="sxs-lookup"><span data-stu-id="2192d-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="2192d-107">**Deaktivert:** Automatisk oppgradering er deaktivert.</span><span class="sxs-lookup"><span data-stu-id="2192d-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="2192d-108">**Suspendert**: Systemet er ikke lenger kvalifisert til å motta automatiske oppgraderinger.</span><span class="sxs-lookup"><span data-stu-id="2192d-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="2192d-109">Du kan ikke konfigurere denne verdien. det er satt av systemet.</span><span class="sxs-lookup"><span data-stu-id="2192d-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="2192d-110">Hvis du vil ha mer informasjon, kan du se [Automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="2192d-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="2192d-111">Hvis du vil laste ned den nyeste [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)versjonen av Azure AD Connect, går du til .</span><span class="sxs-lookup"><span data-stu-id="2192d-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
