---
title: Automatisk opprydding av foreldede enheter i Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555225"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="dbd2c-102">Automatisk opprydding av foreldede enheter i Intune</span><span class="sxs-lookup"><span data-stu-id="dbd2c-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="dbd2c-103">Intune gjør det mulig for administratoren å konfigurere et tidsintervall mellom 90 og 270 dager, hvoretter foreldede enheter fjernes fra tjenesten.</span><span class="sxs-lookup"><span data-stu-id="dbd2c-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="dbd2c-104">Denne innstillingen er organisasjonen bred og når aktivert trer i kraft umiddelbart.</span><span class="sxs-lookup"><span data-stu-id="dbd2c-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="dbd2c-105">Alle enheter som ikke er sjekket inn på Intune-serveren i en periode som overskrider innstillingen, slettes permanent.</span><span class="sxs-lookup"><span data-stu-id="dbd2c-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="dbd2c-106">**Merk at** Bare MDM-enhetsobjekter er kvalifisert for denne oppryddingshandlingen.</span><span class="sxs-lookup"><span data-stu-id="dbd2c-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="dbd2c-107">EAS er bare enhetsobjekter som er utelukket.</span><span class="sxs-lookup"><span data-stu-id="dbd2c-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="dbd2c-108">Hvis du vil ha mer informasjon om når en enhet blir kvalifisert for sletting basert på opprydningsinnstillingen for enheten og "tilstand":</span><span class="sxs-lookup"><span data-stu-id="dbd2c-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="dbd2c-109">Innstilling: **Slett enheter etter siste innsjekkingsdato: Ja (noe verdi (N) i angitte dager)**</span><span class="sxs-lookup"><span data-stu-id="dbd2c-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="dbd2c-110">Basert på verdien (N) som er konfigurert i innstillingen, sletter Intune-tjenesten enheten i de angitte dagene etter at den sist ble kontrollert.</span><span class="sxs-lookup"><span data-stu-id="dbd2c-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="dbd2c-111">Innstilling: **Slett enheter etter siste innsjekkingsdato: Nei**</span><span class="sxs-lookup"><span data-stu-id="dbd2c-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="dbd2c-112">180 dager etter at enhetssertifikatet utløper og ikke fornyes, slettes enheten.</span><span class="sxs-lookup"><span data-stu-id="dbd2c-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="dbd2c-113">**Merk at** I begge tilfeller må enheten registreres i Intune.</span><span class="sxs-lookup"><span data-stu-id="dbd2c-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="dbd2c-114">Registrering skjer under den første enhetskontrollen med Intune-tjenesten.</span><span class="sxs-lookup"><span data-stu-id="dbd2c-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="dbd2c-115">Hvis en enhet registrerer seg for å være på Intune, men ikke blir Intune registrert, slettes enheten 270 dager etter registrering.</span><span class="sxs-lookup"><span data-stu-id="dbd2c-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="dbd2c-116">(90 dager for å merke enheten som tilbakekalt, og deretter ytterligere 180 dager til å slette posten.)</span><span class="sxs-lookup"><span data-stu-id="dbd2c-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="dbd2c-117">Det finnes for øyeblikket ingen mekanisme i Intune-konsollen for å opprette utløpsdatoen for enhetssertifiseringen for en gitt enhet.</span><span class="sxs-lookup"><span data-stu-id="dbd2c-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>