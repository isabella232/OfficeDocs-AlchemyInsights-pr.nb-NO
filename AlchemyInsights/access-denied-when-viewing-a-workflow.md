---
title: Ingen tilgang når du viser en arbeids flyt
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688811"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Ingen tilgang når du viser en arbeids flyt

SharePoint 2013-arbeids flyter som prøver å sende en e-postmelding til en SharePoint-gruppe, kan mislykkes med feil meldingen «ingen tilgang» hvis medlemskapet i SharePoint-gruppen ikke er satt til alle.
  
 **Du kan løse dette problemet ved å gjøre følgende:**
  
 1. La alle se medlemmene i SharePoint-gruppen.
  
 2. Fjern SharePoint-gruppen fra til-eller kopi-linjen i e-postmeldingen.
  
 3. Legg til brukerne eksplisitt i til-eller kopi linjen hvis medlemskaps synligheten ikke kan endres for SharePoint-gruppen.
  
Hvis du vil vise flere detaljer, kan du se [http uautorisert til/_vti_bin/Client.SVC/Sp.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  