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
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544872"
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

