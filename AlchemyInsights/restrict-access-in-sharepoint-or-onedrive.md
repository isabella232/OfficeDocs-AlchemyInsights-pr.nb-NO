---
title: Begrens tilgang i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551460"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begrens tilgang i SharePoint eller OneDrive

I SharePoint og OneDrive begrenser du tilgangen til elementer som filer, mapper og lister ved bare å gi tilgang til grupper eller enkeltpersoner du vil ha tilgang til. Som standard arves tillatelser i SharePoint fra høyere opp i hierarkiet. En fil arver derfor tillatelsene fra mappen, som arver tillatelsene fra biblioteket, som arver tillatelsene fra området.
  
Du kan dele på et høyere nivå (for eksempel ved å dele et helt område) og deretter bryte arv hvis du ikke vil dele alle elementene på området. Men vi anbefaler ikke dette fordi det gjør opprettholde tillatelsene mer komplekse og forvirrende i fremtiden. Her er hva du kan gjøre i stedet:
  
- Hvis du for eksempel vil dele alt innholdet i en mappe med unntak av én fil, flytter du denne filen til en ny plassering som ikke er delt.
    
- Hvis du har to undermapper i en mappe, og du vil dele en undermappe med grupper A og B og bare gi tilgang til den andre under mappen, deler du den overordnede mappen med gruppe A og legger til gruppe B i den første under mappen.
    
[Avslutte deling av en fil eller mappe](https://go.microsoft.com/fwlink/?linkid=2008861)
  

