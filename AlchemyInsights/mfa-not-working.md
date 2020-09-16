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
# <a name="issues-with-azure-mfa"></a>Problemer med Azure MFA
Det er et par ting du kan sjekke hvis brukerne ikke kan logge seg på ved hjelp av godkjenning med flere faktorer (MFA)

1. Den berørte brukeren kan være blokkert i Azure Active Directory-portalen. Hvis det er tilfelle, avbrytes godkjennings forsøk for den bestemte brukeren automatisk. [Følg Fremgangs måten i denne artikkelen for å fjerne blokkeringen av dem.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Hvis det ikke var mulig å fjerne blokkeringen av brukeren, eller brukeren ikke er blokkert, kan du prøve å tilbakestille MFA for brukeren, og de vil gå gjennom registrerings prosessen på nytt. [Følg Fremgangs måten i denne artikkelen.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Hvis dette er første gang du aktiverte MFA og brukerne ikke kan logge seg på klienter som ikke er nett lesere, for eksempel Outlook, Skype, og så videre, kanskje ADAL (Active Directory Authentication Library) ikke er aktivert for O365-abonnementet ditt. I dette tilfellet må du koble til Exchange Online PowerShell og kjøre denne cmdleten:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*