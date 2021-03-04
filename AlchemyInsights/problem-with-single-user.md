---
title: Problem med enkeltbruker
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
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430201"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="8cc10-102">Problem med enkeltbruker</span><span class="sxs-lookup"><span data-stu-id="8cc10-102">Problem with single user</span></span>

- <span data-ttu-id="8cc10-103">Brukeren har kanskje ikke blitt klargjort fordi tjenesten ikke har hatt mulighet til å evaluere brukeren ennå.</span><span class="sxs-lookup"><span data-stu-id="8cc10-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="8cc10-104">Se gjennom veiledningen for hvor lang tid klargjøringen tar, i tillegg til fremdriftslinjen på konfigurasjonssiden for klargjøring.</span><span class="sxs-lookup"><span data-stu-id="8cc10-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="8cc10-105">Hvis den stabile tilstanden som er angitt i delen med tilleggsdetaljer er før datoen da brukeren ble opprettet/oppdatert/slettet, betyr det at vi ikke har evaluert brukeren ennå.</span><span class="sxs-lookup"><span data-stu-id="8cc10-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="8cc10-106">I dette scenarioet er det best å vente til klargjøringstjenesten er ferdig.</span><span class="sxs-lookup"><span data-stu-id="8cc10-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="8cc10-107">Vær oppmerksom på at tjenesten vår bare er oppmerksom på endringer til en bruker i kildesystemet (Cloud HR).</span><span class="sxs-lookup"><span data-stu-id="8cc10-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="8cc10-108">Det må være en gyldig endring i kildesystemet for Azure AD for å oppdage endringen og flyte den inn i Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8cc10-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="8cc10-109">Klargjøringstjenesten evaluert brukeren og bestemte at den ikke skal klargjøres:</span><span class="sxs-lookup"><span data-stu-id="8cc10-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="8cc10-110">Hvis du har angitt et attributtbasert filter for å angi poengberegning, må du kontrollere at brukeren oppfyller kriteriene du har angitt.</span><span class="sxs-lookup"><span data-stu-id="8cc10-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="8cc10-111">Hvis brukere allerede finnes i målsystemet og statusen til brukeren i kilde- og måls samsvarer, vil vi ikke gjøre noe mer.</span><span class="sxs-lookup"><span data-stu-id="8cc10-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="8cc10-112">Klargjøringstjenesten prøvde å klargjøre brukeren, og den mislyktes.</span><span class="sxs-lookup"><span data-stu-id="8cc10-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="8cc10-113">Se gjennom fanen feilsøking og anbefalinger i klargjøringsloggene for disse scenariene:</span><span class="sxs-lookup"><span data-stu-id="8cc10-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="8cc10-114">Et nødvendig attributt for brukeren kan mangle lokalt i Active Directory eller Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8cc10-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="8cc10-115">Genereringsreglene userPrincipalName eller sAMAccountName genererer for eksempel ikke den riktige verdien.</span><span class="sxs-lookup"><span data-stu-id="8cc10-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="8cc10-116">Attributtet som samsvarer (vanligvis ansattId), løses ikke til en unik bruker i lokal Active Directory eller Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8cc10-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="8cc10-117">Det er for eksempel to brukere med samme ansatt-ID i AD, og tjenesten returnerer en feilkode som angir dupliserte måloppføringer for samme kildeoppføring.</span><span class="sxs-lookup"><span data-stu-id="8cc10-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="8cc10-118">Hvis du vil se gjennom logger for enkeltbrukere og grupper, kan du se se gjennom [klargjøringsloggene for et problem med en bestemt bruker.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)</span><span class="sxs-lookup"><span data-stu-id="8cc10-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
