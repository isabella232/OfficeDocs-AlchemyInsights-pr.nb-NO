---
title: Opprette et område i SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199282"
---
# <a name="create-sharepoint-sites-using-templates"></a>Opprette SharePoint-områder ved hjelp av maler

SharePoint-områdemaler er forhåndsbygde definisjoner utviklet rundt bestemte forretningsbehov. Hvis du vil ha mer informasjon, se [bruke maler for å opprette ulike typer SharePoint-områder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Her er noen vanlige problemer/løsninger når det gjelder lagring av et område eller en liste som mal i Sharepoint Online. 

**Lagre område-listen mal-knappen er ikke tilgjengelig eller mangler**

Administratorer må tillate egendefinert skript til å aktivere funksjonene for malen. Detaljert fremgangsmåte, eksempler og vurderinger i 

- [Tillate eller forhindre egendefinert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Området lagre som mal-kommandoen støttes ikke og kan forårsake problemer på områder som bruker SharePoint Server-publisering infrastrukturen.

**Områdemalen kan ikke opprettes eller fungerer ikke riktig**

Malen mangler kanskje en [funksjon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , og vil ikke aktivere. Hvis funksjonen ikke er tilgjengelig for å aktivere i gjeldende områdesamling, kan du ikke bruke malen webområde til å opprette et område.

- Kontroller Hvis eventuelle lister eller biblioteker overskrider [Terskelen for listevisning grensen](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) av 5000 varer dette kan hindre opprettelsen av en områdemal.

- Området som bruker for mange ressurser, og derfor områdemalen overskrider grensen på 50 MB.


- Det er problemer med å vise data fra en liste som bruker en oppslagskolonne. Hvis du vil ha mer informasjon, kan du se [mal-genererte listen ikke viser dataene fra den riktige oppslagslisten i SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).

For mer detaljert informasjon om vanlige problemer og løsninger, se [opprette og bruke maler for webområder](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



