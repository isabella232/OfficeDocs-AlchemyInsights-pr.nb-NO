---
title: Opprette et område i SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770432"
---
# <a name="create-sharepoint-sites-using-templates"></a>Opprette SharePoint-områder ved hjelp av maler

Muligheten til å lagre et nettsted som en mal støttes ikke med moderne kommunikasjons- eller gruppeområder. Hvis du vil ha mer informasjon om hvordan du bruker maler, kan du se [Lagre, laste ned og laste opp et SharePoint-område som en mal](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Her er noen vanlige problemer/løsninger for lagring av et område eller en liste som en mal i Sharepoint Online. 

**Lagre område-/listemal-knappen er ikke tilgjengelig eller mangler**

Administratorer må tillate egendefinert skript for å aktivere malfunksjonene. For detaljerte trinn, eksempler og vurderinger, se 

- [Tillat eller forhindre egendefinert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Kommandoen Lagre område som mal støttes ikke, og kan forårsake problemer på områder som bruker infrastrukturen for Publisering av SharePoint Server.

**Områdemalen kan ikke opprettes eller fungerer ikke på riktig måte**

Malen mangler kanskje en [funksjon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og aktiveres ikke. Hvis funksjonen ikke er tilgjengelig for å aktivere i gjeldende områdesamling, kan du ikke bruke områdemalen til å opprette et område.

- Kontroller om lister eller biblioteker overskrider grenseterskelen for [listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) på 5000 elementer, da dette kan blokkere oppretting av en områdemal.

- Området kan bruke for mange ressurser, og derfor overskrider områdemalen 50 MB grensen.


- Det er problemer med å vise data fra en liste som bruker en oppslagskolonne. Hvis du vil ha mer informasjon, kan du se [Malgenerert liste viser ikke data fra riktig oppslagsliste i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Hvis du vil ha mer detaljert informasjon om vanlige problemer og løsninger, kan du sjekke [Opprette og bruke nettstedsmaler](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



