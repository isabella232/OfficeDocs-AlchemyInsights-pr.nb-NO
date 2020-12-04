---
title: Bruke sikkerhets planer for Microsoft Intune til å konfigurere Windows 10-enheter
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573536"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="5a9ed-102">Bruke sikkerhets planer for Microsoft Intune til å konfigurere Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="5a9ed-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="5a9ed-103">Sikkerhets opprinnelige planer for Intune bidrar til å beskytte brukere og enheter.</span><span class="sxs-lookup"><span data-stu-id="5a9ed-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="5a9ed-104">Sikkerhets opprinnelige planer er Windows-innstillinger, forhånds kon figurerte grupper brukes til å bruke en kjent gruppe med innstillinger og standard verdier som anbefales av de aktuelle sikkerhets teamene.</span><span class="sxs-lookup"><span data-stu-id="5a9ed-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="5a9ed-105">Ved å opprette en opprinnelig basis profil i Intune, oppretter du en mal som består av flere profiler for enhets konfigurasjon.</span><span class="sxs-lookup"><span data-stu-id="5a9ed-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="5a9ed-106">Når du distribuerer sikkerhets opprinnelige planer til grupper av brukere eller enheter, gjelder innstillingene for enheter som kjører på Windows 10 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="5a9ed-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="5a9ed-107">MDM-sikkerhet for sikkerhets plan automatisk (1) aktiverer for eksempel BitLocker for flyttbare stasjoner (2) krever passordet for å låse opp en enhet, og (3) deaktiverer enkel godkjenning.</span><span class="sxs-lookup"><span data-stu-id="5a9ed-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="5a9ed-108">Når en standard verdi ikke fungerer for miljøet ditt, kan du tilpasse den opprinnelige planen for å bruke innstillingene du trenger.</span><span class="sxs-lookup"><span data-stu-id="5a9ed-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="5a9ed-109">Sikkerhets opprinnelige planer bidrar også til å opprette en slutt-til-ende sikker arbeids flyt i Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5a9ed-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="5a9ed-110">Følgende er noen av fordelene med dette:</span><span class="sxs-lookup"><span data-stu-id="5a9ed-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="5a9ed-111">En sikkerhets plan omfatter anbefalte Fremgangs måter og anbefalinger for innstillinger som påvirker sikkerheten.</span><span class="sxs-lookup"><span data-stu-id="5a9ed-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="5a9ed-112">Siden Intune-partnere med Windows-sikkerhetsmaskinvaren som oppretter opprinnelige planer for gruppe policyer, er disse anbefalingene basert på solid veiledning og omfattende opplevelse.</span><span class="sxs-lookup"><span data-stu-id="5a9ed-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="5a9ed-113">Hvis du ikke har brukt Intune og ikke vet hvor du skal begynne, kan sikkerhets opprinnelige planer gjøre det enklere å opprette og distribuere en sikker profil.</span><span class="sxs-lookup"><span data-stu-id="5a9ed-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="5a9ed-114">Hvis du for øyeblikket bruker en gruppe policy, er det mye enklere å overføre til Intune for administrasjons formål, fordi de er innebygd i Intune og inkludere de kuttede funksjonene for administrasjon.</span><span class="sxs-lookup"><span data-stu-id="5a9ed-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="5a9ed-115">Hvis du vil ha mer informasjon, kan du se [sikkerhets opprinnelige planer for Windows](https://go.microsoft.com/fwlink/?linkid=2141503) og [administrasjon av mobil enheter](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="5a9ed-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>