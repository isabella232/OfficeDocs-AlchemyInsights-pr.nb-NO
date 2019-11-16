---
title: Problemer med MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768846"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="cf1c1-102">Problemer med Azure MFA</span><span class="sxs-lookup"><span data-stu-id="cf1c1-102">Issues with Azure MFA</span></span>
<span data-ttu-id="cf1c1-103">Det er et par ting å kontrollere om brukere ikke kan logge på ved hjelp av multi-faktor autentisering (MFA)</span><span class="sxs-lookup"><span data-stu-id="cf1c1-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="cf1c1-104">Den berørte brukeren kan være blokkert i Azure Active Directory-portalen.</span><span class="sxs-lookup"><span data-stu-id="cf1c1-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="cf1c1-105">Hvis det er tilfellet, blir godkjenningsforsøk for den bestemte brukeren automatisk avslått.</span><span class="sxs-lookup"><span data-stu-id="cf1c1-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="cf1c1-106">Følg trinnene i denne artikkelen for å oppheve blokkeringen av dem.</span><span class="sxs-lookup"><span data-stu-id="cf1c1-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="cf1c1-107">Hvis oppheve brukeren ikke hjelpe eller brukeren ikke er blokkert, kan du prøve å tilbakestille MFA for brukeren, og de vil gå gjennom melde prosessen på nytt.</span><span class="sxs-lookup"><span data-stu-id="cf1c1-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="cf1c1-108">Følg trinnene i denne artikkelen.</span><span class="sxs-lookup"><span data-stu-id="cf1c1-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="cf1c1-109">Hvis dette er første gang du aktiverte MFA og brukerne ikke er i stand til å logge inn til ikke-nettleser-klienter som Outlook, Skype, etc, kanskje ADAL (Active Directory Authentication Library) er ikke aktivert på O365 abonnement.</span><span class="sxs-lookup"><span data-stu-id="cf1c1-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="cf1c1-110">I dette tilfellet må du koble til Exchange Online PowerShell og kjøre denne cmdleten:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="cf1c1-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>