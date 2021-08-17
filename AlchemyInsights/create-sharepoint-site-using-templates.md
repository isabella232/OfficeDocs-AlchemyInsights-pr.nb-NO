---
title: Opprette et nettsted i SharePoint Online
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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057975"
---
# <a name="create-sharepoint-sites-using-templates"></a>Opprette SharePoint nettsteder ved hjelp av maler

Muligheten til å lagre et nettsted som en mal støttes ikke med moderne kommunikasjon eller gruppeområder. For mer informasjon om hvordan du bruker maler, kan du se [Lagre, laste ned og laste opp et SharePoint-nettsted som en mal](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Her er noen vanlige problemer/løsninger angående lagring av et nettsted eller en liste som en mal i Sharepoint Online. 

**Knappen Lagre nettsteds-/listemal er ikke tilgjengelig eller mangler**

Administratorer må tillate egendefinert skript for å aktivere malfunksjonene. Hvis du vil ha detaljerte trinn, kan du se eksempler og hensyn 

- [Tillate eller forhindre egendefinert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Kommandoen Lagre område som mal støttes ikke og kan føre til problemer på områder som bruker SharePoint Server-publiseringsinfrastruktur.

**Nettstedsmalen kan ikke opprettes eller fungerer ikke som den skal**

Malen mangler kanskje en [funksjon og](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) aktiveres ikke. Hvis funksjonen ikke er tilgjengelig for å aktivere i den gjeldende nettstedsamlingen, kan du ikke bruke nettstedmalen til å opprette et nettsted.

- Kontroller om det finnes noen lister eller biblioteker som overskrider [terskelen for listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) på 5 000 elementer, for det kan blokkere opprettelsen av en nettstedmal.

- Det kan hende nettstedet bruker for mange ressurser, og derfor overskrider nettstedsmalen grensen på 50 MB.


- Det er problemer med visning av data fra en liste som bruker en oppslagskolonne. For mer informasjon, kan du se [Malgenerert liste viser ikke data fra riktig oppslagsliste i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Hvis du vil ha mer detaljert informasjon om vanlige problemer og løsninger, kan du [se Opprette og bruke nettstedsmaler](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



