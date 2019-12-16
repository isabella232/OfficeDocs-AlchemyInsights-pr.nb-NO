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
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052478"
---
# <a name="create-sharepoint-sites-using-templates"></a>Opprette SharePoint-områder ved hjelp av maler

Maler for SharePoint-områder er forhåndsbygde definisjoner som er utformet rundt et bestemt forretningsbehov. Hvis du vil ha mer informasjon, se [bruke maler til å opprette ulike typer SharePoint-områder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Her er noen vanlige problemer/løsninger i forbindelse med lagring av et område eller en liste som en mal i SharePoint Online. 

**Knappen Lagre område/liste mal er ikke tilgjengelig eller mangler**

Administratorer må tillate egendefinert skript for å aktivere mal funksjonene. For detaljerte trinn, eksempler og betraktninger se 

- [Tillate eller forhindre egendefinert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Kommandoen Lagre område som mal støttes ikke, og kan forårsake problemer på områder som bruker infrastruktur for SharePoint Server-publisering.

**Områdemalen kan ikke opprettes eller fungerer ikke som den skal**

Malen mangler kanskje en [funksjon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) og vil ikke aktivere. Hvis funksjonen ikke er tilgjengelig for aktivering i gjeldende områdesamling, kan du ikke bruke områdemalen til å opprette et område.

- Kontroller om noen lister eller biblioteker overskrider [terskelen for liste visningsgrense](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) for 5000 elementer, da dette kan blokkere oppretting av en områdemal.

- Området bruker kanskje for mange ressurser, og derfor overskrider områdemalen grensen på 50 MB.


- Det er problemer med å vise data fra en liste som bruker en oppslagskolonne. Hvis du vil ha mer informasjon, kan [du se mal-generert liste viser ikke data fra den riktige oppslagslisten i SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Hvis du vil ha mer detaljert informasjon om vanlige problemer og løsninger, kan du se [opprette og bruke områdemaler](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



