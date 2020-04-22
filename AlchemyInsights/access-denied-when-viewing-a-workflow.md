---
title: Ingen tilgang når du viser en arbeidsflyt
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687339"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Ingen tilgang når du viser en arbeidsflyt

SharePoint 2013 arbeidsflyter som prøver å sende en e-post til en SharePoint-gruppe, kan mislykkes med feilmeldingen "Ingen tilgang" hvis medlemskapet i SharePoint-gruppen ikke er satt til Alle.
  
 **Hvis du vil løse dette problemet, gjør du følgende:**
  
 1. La alle se medlemmene av SharePoint-gruppen.
  
 2. Fjern SharePoint-gruppen fra Til- eller KOPI-linjen i e-posten.
  
 3. Legg eksplisitt til brukerne på til- eller KOPI-linjen hvis ansvarssynligheten ikke kan endres for SharePoint-gruppen.
  
Hvis du vil vise flere detaljer, kan du se [HTTP uautorisert til /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  