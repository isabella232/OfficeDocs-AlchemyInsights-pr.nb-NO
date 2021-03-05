---
title: Klargjøring av arbeidsdager til AD-bruker går i karantenetilstand
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
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481880"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="3e50f-102">Klargjøring av arbeidsdager til AD-bruker går i karantenetilstand</span><span class="sxs-lookup"><span data-stu-id="3e50f-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="3e50f-103">**Klargjøring av arbeidsdager til AD-bruker går i karantenetilstand, og ingen brukere opprettes i AD**</span><span class="sxs-lookup"><span data-stu-id="3e50f-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="3e50f-104">Klargjøringsjobben for arbeidsdagen til AD-bruker er satt i karantene, og overvåkingsloggene viser eksportfeilhendelser med **feilmeldingsfeilen: OperationsError-SvcErr: Det oppstod en operasjonsfeil. Ingen overordnet referanse er konfigurert for katalogtjenesten. Katalogtjenesten kan derfor ikke utstede henvisninger til objekter utenfor denne skogen.**</span><span class="sxs-lookup"><span data-stu-id="3e50f-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="3e50f-105">Denne feilen vises vanligvis hvis organisasjonsenheten for Active Directory-beholder ikke er riktig angitt, eller hvis det er problemer med uttrykkstilordningen som brukes for **parentDistinguishedName.**</span><span class="sxs-lookup"><span data-stu-id="3e50f-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="3e50f-106">Se etter skrivefeil i **parameteren** Standard organisasjonsenheten for nye brukere.</span><span class="sxs-lookup"><span data-stu-id="3e50f-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="3e50f-107">Kontroller at den angitte organisasjonsenheten allerede finnes i AD.</span><span class="sxs-lookup"><span data-stu-id="3e50f-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="3e50f-108">Hvis du bruker **parentDistinguishedName** i attributttilordningen, må du kontrollere at det alltid evalueres til en kjent beholder innenfor AD-domenet.</span><span class="sxs-lookup"><span data-stu-id="3e50f-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="3e50f-109">Kontroller Eksport-hendelsen i overvåkingsloggene for å se den genererte verdien.</span><span class="sxs-lookup"><span data-stu-id="3e50f-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="3e50f-110">Hvis du vil ha mer informasjon om hvordan du konfigurerer arbeidsdag for automatisert klargjøring, kan du se [Opplæring: Konfigurere arbeidsdag for automatisk klargjøring av brukere.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="3e50f-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

