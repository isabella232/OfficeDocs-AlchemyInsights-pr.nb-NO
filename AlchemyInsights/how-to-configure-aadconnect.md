---
title: 646 Hvordan du konfigurerer AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722572"
---
# <a name="configure-sync-features"></a><span data-ttu-id="f83d4-102">Konfigurere synkroniseringsfunksjoner</span><span class="sxs-lookup"><span data-stu-id="f83d4-102">Configure sync features</span></span>

<span data-ttu-id="f83d4-103">Azure AD Connect inneholder flere funksjoner som er aktivert som standard, eller som du kan aktivere senere.</span><span class="sxs-lookup"><span data-stu-id="f83d4-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="f83d4-104">Noen funksjoner krever ekstra konfigurasjon i bestemte miljøer.</span><span class="sxs-lookup"><span data-stu-id="f83d4-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="f83d4-105">[Filtrering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) begrenser objektene synkroniseres til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f83d4-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="f83d4-106">Som standard synkroniseres alle brukere, kontakter, grupper og Windows 10-datamaskinkontoer.</span><span class="sxs-lookup"><span data-stu-id="f83d4-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="f83d4-107">Du kan inkludere eller utelate objekter basert på domener, ouer eller andre attributter.</span><span class="sxs-lookup"><span data-stu-id="f83d4-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="f83d4-108">[Synkronisering av passordhash](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkroniserer passordhashen fra den lokale Active Directory til Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f83d4-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="f83d4-109">Dette tillater passordbehandling på ett sted, men bruk av det samme passordet i både lokale og skymiljøer.</span><span class="sxs-lookup"><span data-stu-id="f83d4-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="f83d4-110">Fordi Active Directory er den autoritative kilden, kan du bruke dine egne passordpolicyer.</span><span class="sxs-lookup"><span data-stu-id="f83d4-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="f83d4-111">[Selvbetjent tilbakestilling av passord (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) gjør det mulig for brukere å tilbakestille sine egne passord i skyen mens de fortsatt bruker den lokale passordpolicyen.</span><span class="sxs-lookup"><span data-stu-id="f83d4-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="f83d4-112">[Enhetswriteback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) gjør at registrerte enheter i Azure AD kan skrives tilbake til den lokale Active Directory, slik at de kan brukes til betinget tilgang.</span><span class="sxs-lookup"><span data-stu-id="f83d4-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="f83d4-113">[Forhindre utilsiktet sletting](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) er aktivert som standard for å forhindre for mange samtidige objektslettinger (mer enn 500 objekter per synkronisering).</span><span class="sxs-lookup"><span data-stu-id="f83d4-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="f83d4-114">Du kan endre denne innstillingen for å dekke behovene til organisasjonen.</span><span class="sxs-lookup"><span data-stu-id="f83d4-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="f83d4-115">[Automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) er aktivert som standard for ekspressinstallasjoner og bidrar til å sikre at din versjon av Azure AD Connect alltid er oppdatert.</span><span class="sxs-lookup"><span data-stu-id="f83d4-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
