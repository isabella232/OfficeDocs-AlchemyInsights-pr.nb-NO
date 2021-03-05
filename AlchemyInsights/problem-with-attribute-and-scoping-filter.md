---
title: Problem med attributt- og målfilter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481896"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="ead13-102">Problem med attributt- og målfilter</span><span class="sxs-lookup"><span data-stu-id="ead13-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="ead13-103">**Problem med motstridende UPN-verdier**</span><span class="sxs-lookup"><span data-stu-id="ead13-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="ead13-104">Arbeidsdagen til AD-bruker klargjøring av arbeidsdagen til AD-bruker klargjøring viser feilmeldingen **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique.**</span><span class="sxs-lookup"><span data-stu-id="ead13-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="ead13-105">Operasjonen mislyktes fordi UPN-verdien som er angitt for tillegg/endring, ikke er unik skogsdekkende.</span><span class="sxs-lookup"><span data-stu-id="ead13-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="ead13-106">Feildetaljer: **CONSTRAINT_ATT_TYPE - userPrincipalName.**</span><span class="sxs-lookup"><span data-stu-id="ead13-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="ead13-107">**UserPrincipalName-verdien** som Workday-koblingen prøver å angi når du oppretter AD-brukerkontoen, finnes allerede i AD-måldomenet.</span><span class="sxs-lookup"><span data-stu-id="ead13-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="ead13-108">Dette betyr at enten (1) brukeren allerede finnes og den samsvarende ID-kontrollen mislyktes for brukeren, eller (2) genererte UPN-genereringsregelen en motstridende verdi.</span><span class="sxs-lookup"><span data-stu-id="ead13-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="ead13-109">Her er de foreslåtte løsningstrinnene:</span><span class="sxs-lookup"><span data-stu-id="ead13-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="ead13-110">Hvis brukeren allerede finnes og den samsvarende ID-kontrollen ikke kunne koble arbeidsdagkontoen til Active Directory-kontoen, må du kontrollere om det samsvarende ID-attributtet (vanligvis **ansattID)** i både Arbeidsdag og AD har et nøyaktig samsvar.</span><span class="sxs-lookup"><span data-stu-id="ead13-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="ead13-111">Hvis de ikke har noen treff, er det et dataproblem som må løses.</span><span class="sxs-lookup"><span data-stu-id="ead13-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="ead13-112">Hvis for eksempel AnsattID i arbeidsdag er 001052 og i AD er det 1052, vil klargjøringsmotoren ikke koble de to kontoene og vil prøve å opprette en bruker som allerede finnes.</span><span class="sxs-lookup"><span data-stu-id="ead13-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="ead13-113">Løsningen i dette tilfellet er å endre **AnsattID-verdien** i AD til å inkludere foranstilte nuller for å gjøre den til 001052.</span><span class="sxs-lookup"><span data-stu-id="ead13-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="ead13-114">Hvis det UPN-genererende uttrykket ikke genererer en unik verdi, kan du vurdere å bruke funksjonen **SelectUniqueValue** for dekopiering til å generere en unik verdi hver gang.</span><span class="sxs-lookup"><span data-stu-id="ead13-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="ead13-115">**Arbeidsdag til AD-klargjøring av bruker angir ikke noe lederattributtverdi for AD-brukerkonto**</span><span class="sxs-lookup"><span data-stu-id="ead13-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="ead13-116">Jobben for klargjøring av ad-bruker  for arbeidsdagen angir ikke lederens attributtverdi for AD-brukerkontoer.</span><span class="sxs-lookup"><span data-stu-id="ead13-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="ead13-117">Det finnes to mulige scenarier når denne virkemåten vises:</span><span class="sxs-lookup"><span data-stu-id="ead13-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="ead13-118">Den overordnede i arbeidsdagen kan ikke løses til en tilsvarende AD-brukerkonto fordi den overordnede ikke er i omfanget.</span><span class="sxs-lookup"><span data-stu-id="ead13-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="ead13-119">I et **scenario med flere AD-domener** finnes ikke den overordnede i Workday i samme domene som brukeren.</span><span class="sxs-lookup"><span data-stu-id="ead13-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="ead13-120">Prøv disse trinnene for å løse problemet:</span><span class="sxs-lookup"><span data-stu-id="ead13-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="ead13-121">Hvis du har definert omfangsfiltre, må du først kontrollere om den overordnede er i omfang, og at den oppfyller omfangssetningen.</span><span class="sxs-lookup"><span data-stu-id="ead13-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="ead13-122">Hvis den overordnede ikke oppfyller omfangsfilteret, endrer du filteret slik at den overordnede også beskjærer klargjøringsoperasjonen.</span><span class="sxs-lookup"><span data-stu-id="ead13-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="ead13-123">Hvis du har flere AD-domener, har koblingen en kjent begrensning av manglende evne til å løse referanser på tvers av domenebehandling.</span><span class="sxs-lookup"><span data-stu-id="ead13-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="ead13-124">Hvis du vil ha mer informasjon om hvordan du konfigurerer arbeidsdag for automatisert klargjøring, kan du se [Opplæring: Konfigurere arbeidsdag for automatisk klargjøring av brukere.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="ead13-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













