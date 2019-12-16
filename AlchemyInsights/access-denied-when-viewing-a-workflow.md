---
title: Ingen tilgang når du viser en arbeidsflyt
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050534"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Ingen tilgang når du viser en arbeidsflyt

SharePoint 2013 arbeidsflyter som prøver å sende en e-post til en SharePoint-gruppe kan mislykkes med feilmeldingen "ingen tilgang" Hvis medlemskapet i SharePoint-gruppen ikke er satt til alle.
  
 **Hvis du vil løse dette problemet, gjør du følgende:**
  
 1. Tillat alle å se medlemmene av SharePoint-gruppen.
  
 2. Fjern SharePoint-gruppen fra til-eller kopi-linjen i e-postmeldingen.
  
 3. Legg til brukerne eksplisitt i til-eller kopi-linjen hvis medlemskaps synligheten ikke kan endres for SharePoint-gruppe.
  
For å se flere detaljer henvises det til [http uautorisert til/_vti_bin/Client.SVC/Sp.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  