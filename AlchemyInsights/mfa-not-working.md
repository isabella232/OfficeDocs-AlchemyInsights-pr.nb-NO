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
# <a name="issues-with-azure-mfa"></a>Problemer med Azure MFA
Det er et par ting å kontrollere om brukere ikke kan logge på med godkjenning med flere faktorer (MFA)

1. Den berørte brukeren kan være blokkert i Azure Active Directory-portalen. Hvis dette er tilfellet, blir godkjenningsforsøk for den bestemte brukeren automatisk avslått. [Følg fremgangsmåten i denne artikkelen for å oppheve blokkeringen av dem.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Hvis blokkeringen av brukeren ikke hjalp eller brukeren ikke er blokkert, kan du prøve å tilbakestille MFA for brukeren, og de vil gå gjennom registreringsprosessen på nytt. [Følg fremgangsmåten i denne artikkelen.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Hvis dette er første gang du aktiverte MFA og brukerne ikke kan logge på klienter som ikke er nettlesere, for eksempel Outlook, Skype og så videre, er kanskje ikke ADAL (Active Directory Authentication Library) aktivert på O365-abonnementet. I dette tilfellet må du koble til Exchange Online Powershell og kjøre denne cmdleten:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*