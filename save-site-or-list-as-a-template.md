---
title: Lagre området eller listen som en mal
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 56c52c73e752414d66785f175c3a0e2925ad41c1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/02/2019
ms.locfileid: "31044013"
---
# <a name="save-site-or-list-as-a-template"></a>Lagre området eller listen som en mal

SharePoint-områdemaler er forhåndsbygde definisjoner utviklet rundt bestemte forretningsbehov. Hvis du vil ha mer informasjon, se [bruke maler for å opprette ulike typer SharePoint-områder](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Her er noen vanlige problemer/løsninger når det gjelder lagring av et område eller en liste som mal i SharePoint Online.

**Lagre område-listen mal-knappen er ikke tilgjengelig eller mangler**. 

- Administratorer må tillate egendefinert skript til å aktivere funksjonene for malen. For en detaljert fremgangsmåte, eksempler og vurderinger for å se [Tillat eller forby egendefinert skript](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).


- Området lagre som mal-kommandoen støttes ikke og kan forårsake problemer på områder som bruker SharePoint Server-publisering infrastrukturen.


**Områdemalen kan ikke opprettes eller fungerer ikke riktig**

- Malen mangler kanskje en [funksjon](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , og vil ikke aktivere. Hvis funksjonen ikke er tilgjengelig for å aktivere i gjeldende områdesamling, kan du ikke bruke malen webområde til å opprette et område.


- Kontroller Hvis eventuelle lister eller biblioteker overskrider [Terskelen for listevisning grensen](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) av 5000 varer dette kan hindre opprettelsen av en områdemal.


- Området som bruker for mange ressurser, og derfor områdemalen overskrider grensen på 50 megabyte (MB).


- Det er problemer med å vise data fra en liste som bruker en oppslagskolonne. Hvis du vil ha mer informasjon, kan du se [mal-genererte listen ikke viser dataene fra den riktige oppslagslisten i SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).


Vennligst referanse, [opprette og bruke maler](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)for mer detaljert informasjon om vanlige problemer og løsninger.

