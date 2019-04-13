---
title: 646 hvordan du konfigurerer AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/13/2019
ms.locfileid: "31856665"
---
# <a name="configure-sync-features"></a><span data-ttu-id="b43ac-102">Konfigurere synkroniseringsfunksjoner</span><span class="sxs-lookup"><span data-stu-id="b43ac-102">Configure sync features</span></span>

<span data-ttu-id="b43ac-103">Koble til Azure AD inneholder flere funksjoner som er aktivert som standard, eller som du kan aktivere senere.</span><span class="sxs-lookup"><span data-stu-id="b43ac-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="b43ac-104">Noen funksjoner krever mer konfigurasjon i bestemte miljøer.</span><span class="sxs-lookup"><span data-stu-id="b43ac-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="b43ac-105">[Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) grenser objektene synkroniseres Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b43ac-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="b43ac-106">Som standard, alle brukere, kontakter, grupper og Windows 10 synkroniseres datamaskinkontoer.</span><span class="sxs-lookup"><span data-stu-id="b43ac-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="b43ac-107">Du kan inkludere eller utelate objekter basert på domener, organisasjonsenheter eller andre attributter.</span><span class="sxs-lookup"><span data-stu-id="b43ac-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="b43ac-108">[Passord hash synkroniseringen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserer passord hash-koden fra den lokale Active Directory til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="b43ac-108">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="b43ac-109">Dette gjør at passordadministrasjon på ett sted, men bruk av samme passord i både lokale og sky miljøer.</span><span class="sxs-lookup"><span data-stu-id="b43ac-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="b43ac-110">Active Directory er den autoritative kilden, kan du bruke dine egne passordpolicyer for.</span><span class="sxs-lookup"><span data-stu-id="b43ac-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="b43ac-111">[Self service for å tilbakestille passord (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) , lar brukerne tilbakestiller sine egne passord i skyen under fortsatt bruk av den lokale policyen.</span><span class="sxs-lookup"><span data-stu-id="b43ac-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="b43ac-112">[Enheten writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) tillater registrerte enheter i Azure AD skrives tilbake til den lokale Active Directory slik at de kan brukes for betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="b43ac-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="b43ac-113">[Forhindre utilsiktet slettinger](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) er aktivert som standard for å unngå for mange samtidige objektet slettinger (mer enn 500 objekter per synkronisering).</span><span class="sxs-lookup"><span data-stu-id="b43ac-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="b43ac-114">Du kan endre denne innstillingen for å dekke behovene til organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="b43ac-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="b43ac-115">[Automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er aktivert som standard for express installasjoner og bidrar til å sikre din versjon av Azure AD koble alltid er oppdatert.</span><span class="sxs-lookup"><span data-stu-id="b43ac-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
