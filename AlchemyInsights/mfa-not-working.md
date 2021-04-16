---
title: Problemer med MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810493"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="49139-102">Problemer med Azure MFA</span><span class="sxs-lookup"><span data-stu-id="49139-102">Issues with Azure MFA</span></span>
<span data-ttu-id="49139-103">Det er et par ting å kontrollere om brukere ikke kan logge på med godkjenning med flere faktorer (MFA)</span><span class="sxs-lookup"><span data-stu-id="49139-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="49139-104">Den berørte brukeren kan være blokkert i Azure Active Directory-portalen.</span><span class="sxs-lookup"><span data-stu-id="49139-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="49139-105">Hvis dette er tilfellet, blir godkjenningsforsøk for den bestemte brukeren automatisk avslått.</span><span class="sxs-lookup"><span data-stu-id="49139-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="49139-106">Følg fremgangsmåten i denne artikkelen for å oppheve blokkeringen av dem.</span><span class="sxs-lookup"><span data-stu-id="49139-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="49139-107">Hvis blokkeringen av brukeren ikke hjalp eller brukeren ikke er blokkert, kan du prøve å tilbakestille MFA for brukeren, og de vil gå gjennom registreringsprosessen på nytt.</span><span class="sxs-lookup"><span data-stu-id="49139-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="49139-108">Følg fremgangsmåten i denne artikkelen.</span><span class="sxs-lookup"><span data-stu-id="49139-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="49139-109">Hvis dette er første gang du aktiverte MFA og brukerne ikke kan logge på klienter som ikke er nettlesere, for eksempel Outlook, Skype og så videre, er kanskje ikke ADAL (Active Directory Authentication Library) aktivert på O365-abonnementet.</span><span class="sxs-lookup"><span data-stu-id="49139-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="49139-110">I dette tilfellet må du koble til Exchange Online Powershell og kjøre denne cmdleten:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="49139-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>