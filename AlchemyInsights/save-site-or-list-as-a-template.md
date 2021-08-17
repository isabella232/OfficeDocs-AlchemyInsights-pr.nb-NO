---
title: Lagre nettsted eller liste som en mal
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109213"
---
# <a name="save-site-or-list-as-a-template"></a>Lagre nettsted eller liste som en mal

SharePoint nettstedsmaler er forhåndsbygde definisjoner som er utformet rundt et bestemt forretnings behov. Hvis du vil ha mer informasjon, kan du se Bruke [maler til å opprette forskjellige typer SharePoint nettsteder](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Her er noen vanlige problemer/løsninger angående lagring av et nettsted eller en liste som en mal i SharePoint Online.

**Knappen Lagre nettsteds-/listemal er ikke tilgjengelig eller mangler**. 

- Administratorer må tillate egendefinert skript for å aktivere malfunksjonene. Hvis du vil ha detaljerte trinn, kan du se Tillate [eller forhindre egendefinert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Kommandoen Lagre område som mal støttes ikke og kan føre til problemer på områder som bruker SharePoint Server-publiseringsinfrastruktur.


**Nettstedsmalen kan ikke opprettes eller fungerer ikke som den skal**

- Malen mangler kanskje en [funksjon og](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) aktiveres ikke. Hvis funksjonen ikke er tilgjengelig for å aktivere i den gjeldende nettstedsamlingen, kan du ikke bruke nettstedmalen til å opprette et nettsted.


- Kontroller om det finnes noen lister eller biblioteker som overskrider [terskelen for listevisning](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) på 5 000 elementer, for det kan blokkere opprettelsen av en nettstedmal.


- Området bruker kanskje for mange ressurser, og nettstedsmalen overskrider derfor grensen på 50 megabyte (MB).


- Det er problemer med visning av data fra en liste som bruker en oppslagskolonne. Hvis du vil ha mer informasjon, kan du se [Malgenerert liste](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)viser ikke data fra riktig oppslagsliste i SharePoint Online .


Hvis du vil ha mer detaljert informasjon om vanlige problemer og løsninger, kan du [se Opprette og bruke nettstedsmaler](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

