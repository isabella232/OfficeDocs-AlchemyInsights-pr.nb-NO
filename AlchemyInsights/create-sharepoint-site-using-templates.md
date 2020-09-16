---
title: Opprette et område i SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732242"
---
# <a name="create-sharepoint-sites-using-templates"></a>Opprette SharePoint-nettsteder ved hjelp av maler

Muligheten til å lagre et område som en mal støttes ikke med moderne kommunikasjons-eller gruppe nett steder. Hvis du vil ha mer informasjon om bruk av maler, kan du se [Lagre, laste ned og laste opp et SharePoint-område som en mal](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)

Her er noen vanlige problemer/løsninger når det gjelder lagring av et område eller en liste som en mal i SharePoint Online. 

**Knappen Lagre område/liste mal er ikke tilgjengelig eller mangler**

Administratorer må tillate egen definert skript for å aktivere mal funksjonene. For detaljerte trinn kan du se eksempler og hensyn. 

- [Tillate eller forhindre egen definert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Kommandoen Lagre område som mal støttes ikke og kan føre til problemer på områder som bruker publiserings infrastrukturen for SharePoint Server.

**Nettsteds malen kan ikke opprettes eller fungerer ikke som den skal**

Det kan hende at malen mangler en [funksjon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og ikke aktiveres. Hvis funksjonen ikke er tilgjengelig for aktivering i gjeldende område samling, kan du ikke bruke nettsteds malen til å opprette et område.

- Kontroller om alle lister eller biblioteker overskrider [terskel verdien for liste visnings grensen](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) på 5000 elementer siden dette kan blokkere oppretting av en nettsteds mal.

- Nettstedet bruker kanskje for mange ressurser, og derfor overskrider nettsteds malen grensen på 50 MB.


- Det er problemer med å vise data fra en liste som bruker en oppslags Kol onnen. Hvis du vil ha mer informasjon, kan du se [mal gener ert liste viser ikke data fra den riktige oppslags listen i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Hvis du vil ha mer detaljert informasjon om vanlige problemer og løsninger, kan du merke av for [Opprett og bruk nettsteds maler](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



