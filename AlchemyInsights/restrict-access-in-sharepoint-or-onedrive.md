---
title: Begrense tilgang i SharePoint eller OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383880"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Begrense tilgang i SharePoint eller OneDrive

I SharePoint og OneDrive kan begrense du tilgangen til elementer, for eksempel filer, mapper og lister ved å gi tilgang bare til grupper eller enkeltpersoner som du vil ha tilgang. Som standard tillatelsene i SharePoint, som er arvet fra høyere opp i hierarkiet. Så arver en fil tillatelser fra mappen, som arver tillatelser fra biblioteket, som arver tillatelser fra området.
  
Du kan dele på et høyere nivå (som ved å dele et helt område) og deretter bryte arvingen for, hvis du ikke vil dele alle elementer på området. Men anbefaler vi ikke dette fordi det er å vedlikeholde tillatelser for mer komplekse og forvirrende i fremtiden. Her er hva du kan gjøre i stedet:
  
- Hvis du for eksempel vil dele alt innholdet i en mappe med unntak av én fil i det, kan du flytte filen til en ny plassering som ikke er delt.
    
- Hvis du har to undermapper i en mappe, og du vil dele en undermappe med grupper A og B og tillate bare A gruppetilgang til den andre undermappen, dele den overordnede mappen med gruppe A og legge til gruppe B i den første undermappen.
    
[Avslutte deling av en fil eller mappe](https://go.microsoft.com/fwlink/?linkid=2008861)
  

