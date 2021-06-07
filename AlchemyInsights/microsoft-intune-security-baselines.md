---
title: Bruk Microsoft Intune sikkerhetsgrunnlinjer til å konfigurere Windows 10 enheter
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793895"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="7801a-102">Bruk Microsoft Intune sikkerhetsgrunnlinjer til å konfigurere Windows 10 enheter</span><span class="sxs-lookup"><span data-stu-id="7801a-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="7801a-103">Intune sikkerhetsgrunnlinjer bidrar til å beskytte brukere og enheter.</span><span class="sxs-lookup"><span data-stu-id="7801a-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="7801a-104">Sikkerhetsgrunnlinjer er Windows forhåndskonfigurerte grupper som brukes til å bruke en kjent gruppe med innstillinger og standardverdier som anbefales av de relevante sikkerhetsteamene.</span><span class="sxs-lookup"><span data-stu-id="7801a-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="7801a-105">Når du oppretter en profil for sikkerhetsgrunnlinje i Intune, oppretter du en mal som består av flere profiler for enhetskonfigurasjon.</span><span class="sxs-lookup"><span data-stu-id="7801a-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="7801a-106">Når du distribuerer sikkerhetsgrunnlinjer til grupper av brukere eller enheter, brukes innstillingene på enheter som kjører på Windows 10 eller nyere.</span><span class="sxs-lookup"><span data-stu-id="7801a-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="7801a-107">Sikkerhetsgrunnlinjen for Microsoft Mobile Device Management (MDM) aktiverer for eksempel automatisk BitLocker for flyttbare stasjoner, krever passordet for å låse opp en enhet og deaktiverer grunnleggende godkjenning.</span><span class="sxs-lookup"><span data-stu-id="7801a-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="7801a-108">Når en standardverdi ikke fungerer for miljøet, kan du tilpasse den opprinnelige planen for å bruke innstillingene du trenger.</span><span class="sxs-lookup"><span data-stu-id="7801a-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="7801a-109">Sikkerhetsgrunnlinjer bidrar også til å etablere en ende-til-ende sikker arbeidsflyt i Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7801a-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="7801a-110">En sikkerhetsgrunnlinje inneholder anbefalte fremgangsmåter og anbefalinger for innstillinger som påvirker sikkerheten.</span><span class="sxs-lookup"><span data-stu-id="7801a-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="7801a-111">Intune samarbeider med Windows sikkerhetsteamet som oppretter opprinnelige planer for gruppepolicyer, så disse anbefalingene er basert på solid veiledning og omfattende erfaring.</span><span class="sxs-lookup"><span data-stu-id="7801a-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="7801a-112">Hvis du ikke har brukt Intune før og usikker på hvor du skal begynne, kan sikkerhetsgrunnlinjer hjelpe deg med å opprette og distribuere en sikker profil raskt.</span><span class="sxs-lookup"><span data-stu-id="7801a-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="7801a-113">Hvis du for øyeblikket bruker en gruppepolicy, er det mye enklere å overføre til Intune for administrasjonsformål med sikkerhetsgrunnlinjer fordi de er innebygd i Intune og inkluderer avanserte administrasjonsfunksjoner.</span><span class="sxs-lookup"><span data-stu-id="7801a-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="7801a-114">Hvis du vil ha mer [informasjon, kan du Windows sikkerhetsgrunnlinjer](/windows/security/threat-protection/windows-security-baselines) og [Administrasjon av mobilenheter](/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="7801a-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

