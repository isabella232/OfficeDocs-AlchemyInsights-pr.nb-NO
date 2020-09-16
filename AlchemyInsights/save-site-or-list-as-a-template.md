---
title: Lagre område eller liste som en mal
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727540"
---
# <a name="save-site-or-list-as-a-template"></a>Lagre område eller liste som en mal

SharePoint-nettsteds maler er forhånds bygde definisjoner som er utformet rundt et bestemt forretnings behov. Hvis du vil ha mer informasjon, kan du se [bruke maler til å opprette ulike typer SharePoint-nettsteder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Her er noen vanlige problemer/løsninger når det gjelder lagring av et område eller en liste som en mal i SharePoint Online.

**Knappen Lagre område/liste mal er ikke tilgjengelig eller mangler**. 

- Administratorer må tillate egen definert skript for å aktivere mal funksjonene. For detaljerte trinn kan du se eksempler og hensyn: [tillate eller forhindre egen definerte skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Kommandoen Lagre område som mal støttes ikke og kan føre til problemer på områder som bruker publiserings infrastrukturen for SharePoint Server.


**Nettsteds malen kan ikke opprettes eller fungerer ikke som den skal**

- Det kan hende at malen mangler en [funksjon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og ikke aktiveres. Hvis funksjonen ikke er tilgjengelig for aktivering i gjeldende område samling, kan du ikke bruke nettsteds malen til å opprette et område.


- Kontroller om alle lister eller biblioteker overskrider [terskel verdien for liste visnings grensen](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) på 5000 elementer siden dette kan blokkere oppretting av en nettsteds mal.


- Nettstedet bruker kanskje for mange ressurser, og derfor overskrider nettsteds malen 50 megabyte (MB)-grensen.


- Det er problemer med å vise data fra en liste som bruker en oppslags Kol onnen. Hvis du vil ha mer informasjon, kan du se [mal gener ert liste viser ikke data fra den riktige oppslags listen i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Hvis du vil ha mer detaljert informasjon om vanlige problemer og løsninger, kan du [opprette og bruke nettsteds maler](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

