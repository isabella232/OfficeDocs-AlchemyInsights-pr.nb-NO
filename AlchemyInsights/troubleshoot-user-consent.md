---
title: Feilsøke bruker samtykke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901635"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="2d9a0-102">Feilsøke bruker samtykke</span><span class="sxs-lookup"><span data-stu-id="2d9a0-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="2d9a0-103">Du kan konfigurere hvordan slutt brukere samtykker til programmer gjennom Azure-portalen eller PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2d9a0-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="2d9a0-104">Se [bruker samtykke innstillinger](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for mer informasjon.</span><span class="sxs-lookup"><span data-stu-id="2d9a0-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="2d9a0-105">En administrator kan også bruke [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) til å gi samtykke til delegert tilgang på vegne av en enkelt bruker.</span><span class="sxs-lookup"><span data-stu-id="2d9a0-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="2d9a0-106">Hvis du vil ha mer informasjon, kan du se [få tilgang på vegne av en bruker](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="2d9a0-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="2d9a0-107">[Bruker samtykke feil](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): denne artikkelen omhandler feil som kan oppstå under prosessen med å sendes til et program.</span><span class="sxs-lookup"><span data-stu-id="2d9a0-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="2d9a0-108">Hvis du feil søker ukjente bekreftelser på samtykker som ikke inneholder noen feil meldinger, kan du se [godkjennings scenarioer for Azure ad](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="2d9a0-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>