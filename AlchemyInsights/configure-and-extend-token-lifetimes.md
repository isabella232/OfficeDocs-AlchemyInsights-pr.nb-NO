---
title: Konfigurere og forlenge leve tider for token
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917006"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="986ef-102">Konfigurere og forlenge leve tider for token</span><span class="sxs-lookup"><span data-stu-id="986ef-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="986ef-103">Du kan angi leve tiden til et Access-, SAML-eller ID-token utstedt av Microsoft Identity Platform.</span><span class="sxs-lookup"><span data-stu-id="986ef-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="986ef-104">Du kan angi token-levetid for alle apper i organisasjonen, for et multi-leier (multi-Organization) program eller for en bestemt tjeneste konto i organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="986ef-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="986ef-105">Hvis du vil ha mer informasjon, kan du lese [konfigurerbare token-leve tider](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="986ef-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="986ef-106">Eksempler [på hvordan du kan lese eksempler på hvordan du konfigurerer leve tid for token](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="986ef-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="986ef-107">Hvis du vil lære hvordan du konfigurerer en leve tid og kompatibilitet for et token i Azure Active Directory-B2C (Azure AD B2C), kan du se [konfigurere tokener i Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="986ef-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="986ef-108">Artikkelen [konfigurere virke måten for økten i Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) beskriver metodene for enkel pålogging (SSO) som brukes i Azure ad B2C, og hjelper deg med å velge den mest riktige SSO-metoden når du konfigurerer policyen.</span><span class="sxs-lookup"><span data-stu-id="986ef-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="986ef-109">**Hvor lenge kommer tokener? Hvor lenge er de gyldige for?**</span><span class="sxs-lookup"><span data-stu-id="986ef-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="986ef-110">Token-Lifetime er 1 time og øktens leve tid er 24 timer.</span><span class="sxs-lookup"><span data-stu-id="986ef-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="986ef-111">Dette betyr at hvis det ikke har blitt foretatt noen forespørsler i løpet av 24 timer, må du logge på på nytt før du ber om et nytt token.</span><span class="sxs-lookup"><span data-stu-id="986ef-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="986ef-112">Etter at du har blitt 30, 2020, kan du ikke bruke en ny leier policy for å konfigurere økt-og oppdaterings koder.</span><span class="sxs-lookup"><span data-stu-id="986ef-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="986ef-113">Avgangen skjer innenfor flere måneder etter dette, noe som betyr at vi slutter å føre til eksisterende økt-og oppdaterings kode policyer.</span><span class="sxs-lookup"><span data-stu-id="986ef-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="986ef-114">Du kan fortsatt konfigurere leve tiden for tilgangs token etter utløpet.</span><span class="sxs-lookup"><span data-stu-id="986ef-114">You can still configure access token lifetimes after the deprecation.</span></span>






