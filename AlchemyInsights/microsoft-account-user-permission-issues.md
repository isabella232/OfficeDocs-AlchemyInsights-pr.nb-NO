---
title: Feilsøke problem - Finner ikke brukeren i katalogen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702747"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Feilsøke problem - Finner ikke brukeren i katalogen

Hvis brukere mottar feilmeldingen "finner ikke brukeren" i katalogen, kan du prøve på nytt der problemtypen ikke er bruker i katalogen.

Følgende trinn kan fullføres for å feilsøke problemet.

- Kontroller at kontoen som godtok e-postinvitasjonen, er den samme kontoen som brukes til å logge på senere. Kontroller at brukeren bruker den samme kontoen til å godta invitasjonen og logge på nettstedet. 

Hvis du vil ha mer informasjon, kan du se [Administrere aliaser for Microsoft-kontoen</a> for å administrere Microsoft 365-påloggingen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Bla til hvert område(er) der brukeren mottar feilen. 

Legg til "/_layouts/15/people.aspx/membershipgroupid=0" (innenfor de doble anførselstegn) på slutten av url-adressen for området. 

Eksempel: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Velg brukeren fra listen.

- Klikk **Fjern brukertillatelser** fra båndet. 
-  Legg til brukeren på nytt, og send invitasjonen til brukeren på nytt.

