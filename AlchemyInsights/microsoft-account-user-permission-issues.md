---
title: Feilsøking av problem-brukeren ikke funnet i katalogen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054819"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Feilsøking av problem-brukeren ikke funnet i katalogen

Hvis brukernes får feil beskjed "bruker skrånende ' blir funnet" inne telefonkatalog, behage prøve atter der hvor utsendelsen type er bruker ikke inne adresseliste.

Følgende trinn kan fullføres for å feilsøke problemet.

- Kontroller at kontoen som godtok invitasjonen til e-post, er den samme kontoen som brukes til å logge på senere. Kontroller at brukeren bruker samme konto til å godta invitasjonen og logge på området. 

Hvis du vil ha mer informasjon, kan du se Administrere [aliaser for</a> Microsoft-kontoen din for å administrere Office 365-påloggingen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Bla til hvert område (r) der brukeren mottar feilen. 

Legg til "/_layouts/15/People.aspx/membershipgroupid = 0" (i doble anførselstegn) til slutten av webadressen. 

Eksempel: https://< "Contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Velg brukeren fra listen.

- Klikk **Fjern brukertillatelser** fra båndet. 
-  Legg til brukeren og Send invitasjonen til brukeren på nytt.

