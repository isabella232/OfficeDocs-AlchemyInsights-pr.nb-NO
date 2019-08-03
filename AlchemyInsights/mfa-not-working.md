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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250174"
---
# <a name="issues-with-mfa"></a>Problemer med MFA
Det er et par ting du kan kontrollere om brukere ikke kan logge på ved hjelp av multifaktorautentisering (MFA)

1. Den aktuelle brukeren kan være blokkert i Azure Active Directory Portal. Hvis det er tilfelle, prøver godkjenning for den bestemte brukeren automatisk nektes. [Følg trinnene i denne artikkelen for å fjerne blokkeringen og dermed.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Hvis ikke bidra til å deaktivere blokkering av brukeren eller brukeren ikke er blokkert, kan du prøve å tilbakestille MFA for brukeren og de vil gå gjennom prosessen med registrering på nytt. [Følg trinnene i denne artikkelen.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Hvis dette er første gangen du aktiverte MFA og brukerne ikke kan logge på ikke-weblesere klienter, for eksempel Outlook, Skype og så videre, er kanskje ADAL (Active Directory-godkjenning Library) ikke aktivert på O365-abonnement. I dette tilfellet må du koble til Exchange Online Powershell og kjøre denne cmdleten:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*