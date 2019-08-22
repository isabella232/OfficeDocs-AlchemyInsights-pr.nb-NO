---
title: Ingen tilgang når du viser en arbeidsflyt
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495832"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Ingen tilgang når du viser en arbeidsflyt

SharePoint 2013 arbeidsflyter som forsøker å sende en e-post til en SharePoint-gruppe kan mislykkes med en feilmelding av typen "Ingen tilgang" Hvis medlemskap for SharePoint-gruppen ikke er satt til alle.
  
 **Hvis du vil løse dette problemet, gjør du følgende:**
  
 1. Tillat alle å se medlemmer av SharePoint-gruppen.
  
 2. Fjern SharePoint-gruppen fra til- eller Kopi-linjen i e-postmeldingen.
  
 3. Legge til brukere eksplisitt i til- eller kopi linje hvis medlemskap synligheten ikke kan endres for SharePoint-gruppen.
  
Hvis du vil vise flere detaljer kan du se [HTTP uautorisert til /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  