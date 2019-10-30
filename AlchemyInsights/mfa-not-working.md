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
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768846"
---
# <a name="issues-with-azure-mfa"></a>Problemer med Azure MFA
Det er et par ting å kontrollere om brukere ikke kan logge på ved hjelp av multi-faktor autentisering (MFA)

1. Den berørte brukeren kan være blokkert i Azure Active Directory-portalen. Hvis det er tilfellet, blir godkjenningsforsøk for den bestemte brukeren automatisk avslått. [Følg trinnene i denne artikkelen for å oppheve blokkeringen av dem.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Hvis oppheve brukeren ikke hjelpe eller brukeren ikke er blokkert, kan du prøve å tilbakestille MFA for brukeren, og de vil gå gjennom melde prosessen på nytt. [Følg trinnene i denne artikkelen.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Hvis dette er første gang du aktiverte MFA og brukerne ikke er i stand til å logge inn til ikke-nettleser-klienter som Outlook, Skype, etc, kanskje ADAL (Active Directory Authentication Library) er ikke aktivert på O365 abonnement. I dette tilfellet må du koble til Exchange Online PowerShell og kjøre denne cmdleten:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*