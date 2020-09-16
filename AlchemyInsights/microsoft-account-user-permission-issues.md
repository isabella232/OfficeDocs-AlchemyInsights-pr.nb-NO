---
title: Feilsøke et problem – finner ikke brukeren i katalogen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725416"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Feilsøke et problem – finner ikke brukeren i katalogen

Hvis brukere får feil meldingen «finner ikke brukeren» i katalogen, kan du prøve på nytt der problem typen er bruker som ikke er i katalog.

Følgende trinn kan utføres for å feilsøke problemet.

- Kontroller at kontoen som godtok e-postinvitasjonen, er den samme kontoen som brukes til å logge på senere. Kontroller at brukeren bruker samme konto til å godta invitasjonen og logge på nettstedet. 

Hvis du vil ha mer informasjon, kan du se [hvordan du behandler aliaser for Microsoft-kontoen for </a> å administrere Microsoft 365-påloggingen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Gå til hvert område (r) som brukeren mottar feilen i. 

Legg til «/_layouts/15/People.aspx/membershipgroupid = 0» (i doble anførsels tegn) på slutten av Netta dressen for nettstedet. 

Eksempel: https://< «contoso» >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Velg brukeren fra listen.

- Klikk **Fjern bruker tillatelser** fra båndet. 
-  Legg tilbake brukeren og Send invitasjonen til brukeren på nytt.

