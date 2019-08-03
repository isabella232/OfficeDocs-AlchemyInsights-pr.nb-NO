---
title: Feilsøke problemet - brukeren ble ikke funnet i katalogen
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0909edc581c811fdc4683b004e0df0adbac88d1c
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/26/2019
ms.locfileid: "35249922"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Feilsøke problemet - brukeren ble ikke funnet i katalogen

Hvis brukere får feil melding "brukeren finnes ikke" i katalogen. Prøv på nytt der problemtypen brukeren ikke er i katalogen.

Følgende trinn kan fullføres hvis du vil feilsøke problemet.

- Sikre at kontoen som godkjent e-postinvitasjonen er den samme kontoen som brukes til å logge på igjen senere. Kontroller at du bruker samme konto til å godta invitasjonen og logge inn på området. 

For mer informasjon, se [å administrere aliaser for Microsoft-kontoen</a> til å administrere Office 365-pålogging](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Bla til hver område(r) der brukeren mottar feilen. 

Legge til "/ _layouts/15/people.aspx/membershipgroupid=0" (i de doble anførselstegnene) på slutten av URL-adressen for området. 

Eksempel: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Velg brukeren fra listen.

- Klikk **Fjern brukertillatelser** fra båndet. 
-  Legge tilbake til brukeren, og Send invitasjonen på nytt til brukeren.

