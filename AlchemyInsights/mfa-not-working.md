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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545183"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="72717-102">Problemer med MFA</span><span class="sxs-lookup"><span data-stu-id="72717-102">Issues with MFA</span></span>
<span data-ttu-id="72717-103">Der er et par saker å sjekk hvis brukernes kan ikke logikk benytter mange--faktoren Authentication (MFA)</span><span class="sxs-lookup"><span data-stu-id="72717-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="72717-104">Den berørte brukeren kan være blokkert i Azure Active Directory-portalen.</span><span class="sxs-lookup"><span data-stu-id="72717-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="72717-105">Hvis det er tilfellet, blir godkjenningsforsøk for den bestemte brukeren automatisk avslått.</span><span class="sxs-lookup"><span data-stu-id="72717-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="72717-106">Følg trinnene i denne artikkelen for å oppheve blokkeringen av dem.</span><span class="sxs-lookup"><span data-stu-id="72717-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="72717-107">Hvis oppheve brukeren ikke hjelpe eller brukeren ikke er blokkert, kan du prøve å tilbakestille MFA for brukeren, og de vil gå gjennom melde prosessen på nytt.</span><span class="sxs-lookup"><span data-stu-id="72717-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="72717-108">Følg trinnene i denne artikkelen.</span><span class="sxs-lookup"><span data-stu-id="72717-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="72717-109">Hvis dette er første gang du aktiverte MFA og brukerne ikke er i stand til å logge inn til ikke-nettleser-klienter som Outlook, Skype, etc, kanskje ADAL (Active Directory Authentication Library) er ikke aktivert på O365 abonnement.</span><span class="sxs-lookup"><span data-stu-id="72717-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="72717-110">I dette tilfellet må du koble til Exchange Online PowerShell og kjøre denne cmdleten:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="72717-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>