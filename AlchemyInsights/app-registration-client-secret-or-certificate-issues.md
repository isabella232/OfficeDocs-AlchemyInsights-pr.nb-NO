---
title: Klienthemmelighet for appregistrering eller sertifikatproblemer
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404782"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="a6e7c-102">Klienthemmelighet for appregistrering eller sertifikatproblemer</span><span class="sxs-lookup"><span data-stu-id="a6e7c-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="a6e7c-103">Programklientens hemmelige utløp?</span><span class="sxs-lookup"><span data-stu-id="a6e7c-103">Application client secret expiring?</span></span>

<span data-ttu-id="a6e7c-104">Uavhengig av hvordan det registrerte programmet ble opprettet, enten gjennom standard registreringsprosessen i appregistreringsportalen eller hvis tjenesteprinsippet ble opprettet i leieren ved hjelp av programsamtykke, må en ny klienthemmelighet opprettes før utløpet av den gjeldende og oppdateres i den relaterte programkoden.</span><span class="sxs-lookup"><span data-stu-id="a6e7c-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="a6e7c-105">Den maksimale gyldighetsperioden er 2 år.</span><span class="sxs-lookup"><span data-stu-id="a6e7c-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="a6e7c-106">Som en påminnelse må den hemmelige verdien registreres, da den ikke lenger vil være synlig når du forlater appregistreringssiden i portalen.</span><span class="sxs-lookup"><span data-stu-id="a6e7c-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="a6e7c-107">Hvis du vil ha mer informasjon, kan du se [Hurtigstart: Registrere en app](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) i Microsofts identitetsplattform og Anbefalte fremgangsmåter [for Microsoft-identitetsplattformen.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="a6e7c-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="a6e7c-108">Hvis du vil ha mer informasjon, kan du [se Opprette en Azure AD-app & tjenesteprinsipp i portalen – Microsofts identitetsplattform.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="a6e7c-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
