---
title: 646 slik konfigurerer du AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704498"
---
# <a name="configure-sync-features"></a><span data-ttu-id="ed8e4-102">Konfigurere synkroniserings funksjoner</span><span class="sxs-lookup"><span data-stu-id="ed8e4-102">Configure sync features</span></span>

<span data-ttu-id="ed8e4-103">Azure AD Connect inkluderer flere funksjoner som er aktivert som standard, eller som du kan aktivere senere.</span><span class="sxs-lookup"><span data-stu-id="ed8e4-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="ed8e4-104">Noen funksjoner krever ytterligere konfigurasjon i bestemte miljøer.</span><span class="sxs-lookup"><span data-stu-id="ed8e4-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="ed8e4-105">[Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) begrenser at objektene er synkronisert med Azure ad.</span><span class="sxs-lookup"><span data-stu-id="ed8e4-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="ed8e4-106">Som standard er alle brukere, kontakter, grupper og Windows 10-data maskin kontoer synkronisert.</span><span class="sxs-lookup"><span data-stu-id="ed8e4-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="ed8e4-107">Du kan inkludere eller utelate objekter basert på domener, organisasjons enheter eller andre attributter.</span><span class="sxs-lookup"><span data-stu-id="ed8e4-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="ed8e4-108">[Passord nummer synkronisering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserer passord nummeret fra den lokale Active Directory til Azure ad.</span><span class="sxs-lookup"><span data-stu-id="ed8e4-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="ed8e4-109">Dette gjør det mulig for passord behandling på ett sted, men bruker samme passord i lokale og Sky miljøer.</span><span class="sxs-lookup"><span data-stu-id="ed8e4-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="ed8e4-110">Fordi Active Directory er den autoritative kilden, kan du bruke dine egne passord policyer.</span><span class="sxs-lookup"><span data-stu-id="ed8e4-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="ed8e4-111">[Selv betjent tilbakestilling av passord (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) lar brukere tilbakestille sine egne passord i skyen mens de fremdeles bruker den lokale passord policyen.</span><span class="sxs-lookup"><span data-stu-id="ed8e4-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="ed8e4-112">[Bakgrunns skriving for enheter](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) lar registrerte enheter i Azure ad skrives tilbake til den lokale Active Directory, slik at de kan brukes til betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="ed8e4-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="ed8e4-113">[Unngå utilsiktede](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) slettinger er aktivert som standard for å forhindre for mange samtidige objekt slettinger (mer enn 500 objekter per synkronisering).</span><span class="sxs-lookup"><span data-stu-id="ed8e4-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="ed8e4-114">Du kan endre denne innstillingen for å oppfylle organisasjonens behov.</span><span class="sxs-lookup"><span data-stu-id="ed8e4-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="ed8e4-115">[Automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er aktivert som standard for hurtig installasjoner og hjelper deg med å sikre at din versjon av Azure ad Connect alltid er oppdatert.</span><span class="sxs-lookup"><span data-stu-id="ed8e4-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
