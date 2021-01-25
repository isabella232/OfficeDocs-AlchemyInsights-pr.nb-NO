---
title: API-tillatelser og samtykke
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975000"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="d47a4-102">API-tillatelser og samtykke</span><span class="sxs-lookup"><span data-stu-id="d47a4-102">API permissions and consent</span></span>

<span data-ttu-id="d47a4-103">Programmer som integreres med Microsoft Identity Platform, følger en Autorisasjons modell som gir brukere og administratorer kontroll over hvordan data kan nås.</span><span class="sxs-lookup"><span data-stu-id="d47a4-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="d47a4-104">Implementeringen av Autorisasjons modellen er oppdatert på Microsoft Identity Platform Endpoint.</span><span class="sxs-lookup"><span data-stu-id="d47a4-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="d47a4-105">Den endrer hvordan en app må samhandle med Microsoft Identity Platform.</span><span class="sxs-lookup"><span data-stu-id="d47a4-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="d47a4-106">[Tillatelser og samtykke i Microsoft Identity Platform Endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) dekker de grunnleggende konseptene til denne Autorisasjons modellen, inkludert omfang, tillatelser og samtykke.</span><span class="sxs-lookup"><span data-stu-id="d47a4-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="d47a4-107">[Azure Active Directory (Azure ad) samtykke rammeverk](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) gjør det enkelt å utvikle nett og opprinnelige klient programmer med flere Tenant.</span><span class="sxs-lookup"><span data-stu-id="d47a4-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="d47a4-108">Disse programmene tillater pålogging av bruker kontoer fra en Azure AD-leier som er forskjellig fra den som programmet er registrert i.</span><span class="sxs-lookup"><span data-stu-id="d47a4-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="d47a4-109">Det kan også hende at de trenger tilgang til nett-APIer, for eksempel Microsoft Graph API (for å få tilgang til Azure AD, Intune og tjenester i Microsoft 365) og andre Microsoft Services-APIer, i tillegg til dine egne nett BAS-APIer.</span><span class="sxs-lookup"><span data-stu-id="d47a4-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

