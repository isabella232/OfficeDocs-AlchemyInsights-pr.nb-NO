---
title: Problemer med administrator samtykke
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
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901506"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="0420a-102">Problemer med administrator samtykke</span><span class="sxs-lookup"><span data-stu-id="0420a-102">Admin consent issues</span></span>

1. <span data-ttu-id="0420a-103">Aktiver [arbeids flyten for administrator samtykke](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) for å tillate at brukere ber om administrator godkjenning direkte fra skjerm bildet for samtykke.</span><span class="sxs-lookup"><span data-stu-id="0420a-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="0420a-104">Hvis du eller programmets brukere ser uventede feil under samtykke prosessen, kan du se denne artikkelen for feil søkings trinn: [uventet feil under utføring av samtykke til et program](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="0420a-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="0420a-105">Lær mer om [administrator samtykke på Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), hvordan [samtykke lede teksten](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) fungerer, og hvordan du [evaluerer en forespørsel om godkjennings samtykke for hele leieren](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="0420a-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="0420a-106">Programmer som integreres med Microsoft Identity Platform, følger en Autorisasjons modell som gir brukere og administratorer kontroll over hvordan data kan nås.</span><span class="sxs-lookup"><span data-stu-id="0420a-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="0420a-107">Implementeringen av Autorisasjons modellen er oppdatert på Microsoft Identity Platform Endpoint, og den endrer hvordan en app må samhandle med Microsoft Identity Platform.</span><span class="sxs-lookup"><span data-stu-id="0420a-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="0420a-108">Se [tillatelser og samtykke i Microsoft Identity Platform Endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for en oversikt over denne Autorisasjons modellen, inkludert omfang, tillatelser og samtykke.</span><span class="sxs-lookup"><span data-stu-id="0420a-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>