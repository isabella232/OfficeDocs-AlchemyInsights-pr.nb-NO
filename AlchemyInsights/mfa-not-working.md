---
title: Problemer med MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755140"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="83ee3-102">Problemer med Azure MFA</span><span class="sxs-lookup"><span data-stu-id="83ee3-102">Issues with Azure MFA</span></span>
<span data-ttu-id="83ee3-103">Det er et par ting du kan sjekke hvis brukerne ikke kan logge seg på ved hjelp av godkjenning med flere faktorer (MFA)</span><span class="sxs-lookup"><span data-stu-id="83ee3-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="83ee3-104">Den berørte brukeren kan være blokkert i Azure Active Directory-portalen.</span><span class="sxs-lookup"><span data-stu-id="83ee3-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="83ee3-105">Hvis det er tilfelle, avbrytes godkjennings forsøk for den bestemte brukeren automatisk.</span><span class="sxs-lookup"><span data-stu-id="83ee3-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="83ee3-106">Følg Fremgangs måten i denne artikkelen for å fjerne blokkeringen av dem.</span><span class="sxs-lookup"><span data-stu-id="83ee3-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="83ee3-107">Hvis det ikke var mulig å fjerne blokkeringen av brukeren, eller brukeren ikke er blokkert, kan du prøve å tilbakestille MFA for brukeren, og de vil gå gjennom registrerings prosessen på nytt.</span><span class="sxs-lookup"><span data-stu-id="83ee3-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="83ee3-108">Følg Fremgangs måten i denne artikkelen.</span><span class="sxs-lookup"><span data-stu-id="83ee3-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="83ee3-109">Hvis dette er første gang du aktiverte MFA og brukerne ikke kan logge seg på klienter som ikke er nett lesere, for eksempel Outlook, Skype, og så videre, kanskje ADAL (Active Directory Authentication Library) ikke er aktivert for O365-abonnementet ditt.</span><span class="sxs-lookup"><span data-stu-id="83ee3-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="83ee3-110">I dette tilfellet må du koble til Exchange Online PowerShell og kjøre denne cmdleten:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="83ee3-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>