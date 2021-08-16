---
title: Feilsøke problem – finner ikke brukeren i katalogen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098179"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Feilsøke problem – finner ikke brukeren i katalogen

Hvis brukerne får feilmeldingen «finner ikke brukeren» i katalogen, kan du prøve på nytt der problemtypen ikke er bruker i katalogen.

Følgende trinn kan fullføres for å feilsøke problemet.

- Kontroller at kontoen som godtok e-postinvitasjonen, er den samme kontoen som brukes til å logge på senere. Kontroller at brukeren bruker samme konto til å godta invitasjonen og logge på nettstedet. 

Hvis du vil ha mer informasjon, kan du se Slik administrerer du [aliaser for </a> Microsoft-kontoen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)for å administrere Microsoft 365 pålogging . 

- Bla til hvert nettsted der brukeren mottar feilen. 

Legg til «/_layouts/15/people.aspx/membershipgroupid=0» (i doble anførselstegn) på slutten av nettadressen til nettstedet. 

Eksempel: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Velg brukeren fra listen.

- Klikk **Fjern brukertillatelser** fra båndet. 
-  Legg til brukeren på nytt, og send invitasjonen på nytt til brukeren.

