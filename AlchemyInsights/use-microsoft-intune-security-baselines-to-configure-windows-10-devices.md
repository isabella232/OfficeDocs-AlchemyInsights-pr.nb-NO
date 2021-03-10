---
title: Bruke sikkerhets baselines for Microsoft Intune til å konfigurere Windows 10-enheter
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696376"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="f8e23-102">Bruke sikkerhets baselines for Microsoft Intune til å konfigurere Windows 10-enheter</span><span class="sxs-lookup"><span data-stu-id="f8e23-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="f8e23-103">Sikkerhets baselines for Intune bidrar til å beskytte brukere og enheter.</span><span class="sxs-lookup"><span data-stu-id="f8e23-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="f8e23-104">Sikkerhets baselines are Windows settings's pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span><span class="sxs-lookup"><span data-stu-id="f8e23-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="f8e23-105">Når du oppretter en sikkerhets baseline-profil i Intune, oppretter du en mal som består av flere enhetskonfigurasjonsprofiler.</span><span class="sxs-lookup"><span data-stu-id="f8e23-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="f8e23-106">Når du distribuerer sikkerhets baselines til grupper med brukere eller enheter, brukes innstillingene på enheter som kjører på Windows 10 eller nyere versjoner.</span><span class="sxs-lookup"><span data-stu-id="f8e23-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="f8e23-107">Sikkerhets baseline for administrasjon av mobilenheter (MDM) for Microsoft aktiverer for eksempel automatisk (1) BitLocker for flyttbare stasjoner, (2) krever passordet for å låse opp en enhet, og (3) deaktiverer grunnleggende godkjenning.</span><span class="sxs-lookup"><span data-stu-id="f8e23-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="f8e23-108">Når en standardverdi ikke fungerer for miljøet, kan du tilpasse den opprinnelige planen slik at den bruker innstillingene du trenger.</span><span class="sxs-lookup"><span data-stu-id="f8e23-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="f8e23-109">Sikkerhets baselines also help establish an end-to-end secure workflow in Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f8e23-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="f8e23-110">Her er noen fordeler med denne funksjonaliteten:</span><span class="sxs-lookup"><span data-stu-id="f8e23-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="f8e23-111">En sikkerhets baseline inneholder anbefalte fremgangsmåter og anbefalinger for innstillinger som påvirker sikkerhet.</span><span class="sxs-lookup"><span data-stu-id="f8e23-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="f8e23-112">Fordi Intune samarbeider med Windows-sikkerhetsteamet som oppretter referanselinjer for gruppepolicyer, er disse anbefalingene basert på en solid veiledning og omfattende opplevelse.</span><span class="sxs-lookup"><span data-stu-id="f8e23-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="f8e23-113">Hvis du ikke har brukt Intune før, og du er usikker på hvor du skal begynne, kan sikkerhets baselines hjelpe deg med å opprette og distribuere en sikker profil raskt.</span><span class="sxs-lookup"><span data-stu-id="f8e23-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="f8e23-114">Hvis du for øyeblikket bruker en gruppepolicy, er det mye enklere å overføre til Intune for administrasjonsformål, fordi disse sikkerhets baselines er innebygd i Intune og inkluderer de aller beste funksjonene for administrasjon.</span><span class="sxs-lookup"><span data-stu-id="f8e23-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="f8e23-115">Hvis du vil ha mer informasjon, kan du se [Windows sikkerhets referanselinjer](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) og [administrasjon av mobilenheter.](https://docs.microsoft.com/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="f8e23-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>