---
title: Konfigurere klargjøringstjenesten
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
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482873"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="c89c9-102">Konfigurere klargjøringstjenesten</span><span class="sxs-lookup"><span data-stu-id="c89c9-102">Configuring the Provision service</span></span>

<span data-ttu-id="c89c9-103">For at automatisert klargjøring av bruker skal fungere, krever Azure AD gyldig legitimasjon som tillater at den kobler seg til Workday Web Services API.</span><span class="sxs-lookup"><span data-stu-id="c89c9-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="c89c9-104">I tillegg validerer knappen Test tilkobling på klargjøringsappen for Arbeidsdag til AD-bruker også om den kan koble til klargjøringsagenten for Azure AD Connect knyttet til AD-domenet.</span><span class="sxs-lookup"><span data-stu-id="c89c9-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="c89c9-105">Hvis Azure-portalen returnerer en feil når du lagrer legitimasjonen, følger du de anbefalte trinnene nedenfor:</span><span class="sxs-lookup"><span data-stu-id="c89c9-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="c89c9-106">Kontroller at du har konfigurert brukerkontoen for Workday Integration System som angitt i opplæringsdelen [Konfigurere integrasjonssystembruker i Arbeidsdag.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="c89c9-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="c89c9-107">Kontroller at klargjøringsagenttjenesten for Azure AD Connect er oppe og kjører på den lokale Windows-serveren ved hjelp av tjenestebehandlingskonsollen.</span><span class="sxs-lookup"><span data-stu-id="c89c9-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="c89c9-108">Du kan også kontrollere statusen til agenten i Azure Portal ved å klikke knappen Vis lokale agenter.</span><span class="sxs-lookup"><span data-stu-id="c89c9-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="c89c9-109">Kontroller at du skriver inn verdien for feltet Brukernavn for arbeidsdag ved hjelp av formatet username@workday-tenant-navn.</span><span class="sxs-lookup"><span data-stu-id="c89c9-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="c89c9-110">Hvis navnet på arbeidsdagen-tenanten mangler, mislykkes godkjenningen for arbeidsdagen.</span><span class="sxs-lookup"><span data-stu-id="c89c9-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="c89c9-111">Hvis du konfigurerer integrering med Workday-implementering av tenanten, må du notere deg de planlagte nedetidstimene for Arbeidsdag-leieren.</span><span class="sxs-lookup"><span data-stu-id="c89c9-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="c89c9-112">Arbeidsdagen har planlagt nedsatt tid for implementering av leiere over helger (vanligvis fra fredag kveld til lørdag morgen) og tilkoblingsfeil i dette nedetidsvinduet er et kjent problem som automatisk løses så snart implementeringen av tenantene er tilkoblet igjen.</span><span class="sxs-lookup"><span data-stu-id="c89c9-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="c89c9-113">I sjeldne tilfeller kan du også se denne feilen hvis passordet til integrasjonssystemets bruker endres på grunn av en leieroppdatering, eller hvis kontoen er låst eller har utløpt status.</span><span class="sxs-lookup"><span data-stu-id="c89c9-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="c89c9-114">Kontroller statusen for integrasjonssystemet med workday-administratoren.</span><span class="sxs-lookup"><span data-stu-id="c89c9-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="c89c9-115">Hvis du vil ha mer informasjon om hvordan du konfigurerer arbeidsdag for automatisert klargjøring, kan du se [Opplæring: Konfigurere arbeidsdag for automatisk klargjøring av bruker.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="c89c9-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
