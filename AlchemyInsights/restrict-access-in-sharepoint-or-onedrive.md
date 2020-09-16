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
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720691"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begrense tilgang i SharePoint eller OneDrive

I SharePoint og OneDrive begrenser du tilgang til elementer som filer, mapper og lister ved å gi tilgang bare til grupper eller enkelt personer du vil ha tilgang til. Tillatelser i SharePoint arves som standard fra høyere opp i hierarkiet. Så en fil arver tillatelsene fra mappen, som arver tillatelsene fra biblioteket, som arver tillatelsene fra området.
  
Du kan dele på et høyere nivå (for eksempel ved å dele et helt nettsted) og deretter bryte arv hvis du ikke vil dele alle elementene på området. Vi anbefaler imidlertid ikke dette fordi det gjør det enklere å vedlikeholde tillatelsene mer komplisert og forvirrende i fremtiden. Dette kan du gjøre i stedet:
  
- Hvis du for eksempel vil dele alt innholdet i en mappe bortsett fra én fil i den, flytter du filen til en ny plassering som ikke er delt.
    
- Hvis du har to under mapper i en mappe, og du vil dele én under mappe med grupper A og B og bare gi gruppen tilgang til den andre under mappen, kan du dele den overordnede mappen med grupper A og legge til gruppe B i den første under mappen.
    
[Stoppe deling av en fil eller mappe ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

