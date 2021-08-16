---
title: Begrense tilgang i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075049"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begrense tilgang i SharePoint eller OneDrive

I SharePoint og OneDrive begrenser du tilgangen til elementer som filer, mapper og lister ved å gi tilgang bare til grupper eller enkeltpersoner du vil ha tilgang til. Tillatelser i SharePoint arves som standard fra høyere opp i hierarkiet. En fil arver derfor tillatelsene fra mappen, som arver tillatelsene fra biblioteket, som arver tillatelsene fra nettstedet.
  
Du kan dele på et høyere nivå (for eksempel ved å dele et helt nettsted) og deretter bryte arven hvis du ikke vil dele alle elementene på nettstedet. Vi anbefaler imidlertid ikke dette fordi det gjør vedlikehold av tillatelsene mer komplekse og forvirrende i fremtiden. Dette kan du gjøre i stedet:
  
- Hvis du for eksempel vil dele alt innholdet i en mappe bortsett fra én fil i den, flytter du filen til en ny plassering som ikke er delt.
    
- Hvis du har to undermapper i en mappe, og du vil dele én undermappe med gruppe A og B og bare gi gruppe A tilgang til den andre undermappen, kan du dele den overordnede mappen med gruppe A og legge til gruppe B i den første undermappen.
    
[Slutte å dele en fil eller mappe ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

