---
title: Ingen tilgang når du viser en arbeidsflyt
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: cced887b03876eef527e0166a5a3c9be4b553029
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/24/2019
ms.locfileid: "29481730"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Ingen tilgang når du viser en arbeidsflyt

SharePoint 2013 arbeidsflyter som forsøker å sende en e-post til en SharePoint-gruppe kan mislykkes med en feilmelding av typen "Ingen tilgang" Hvis medlemskap for SharePoint-gruppen ikke er satt til alle.
  
 **Hvis du vil løse dette problemet, gjør du følgende:**
  
 1. Tillat alle å se medlemmer av SharePoint-gruppen. 
  
 2. Fjern SharePoint-gruppen fra til- eller Kopi-linjen i e-postmeldingen. 
  
 3. Legge til brukere eksplisitt i til- eller kopi linje hvis medlemskap synligheten ikke kan endres for SharePoint-gruppen. 
  
Hvis du vil vise flere detaljer kan du se [HTTP uautorisert til /_vti_bin/client.svc/sp.utilities.utility.SendEmail ](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  

