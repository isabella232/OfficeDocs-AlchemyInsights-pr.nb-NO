---
title: Ingen tilgang når du viser en arbeidsflyt
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955210"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Ingen tilgang når du viser en arbeidsflyt

SharePoint 2013 Arbeidsflyter som prøver å sende en e-postmelding til en SharePoint-gruppe, kan mislykkes med feilmeldingen Ingen tilgang hvis medlemskapet i SharePoint-gruppen ikke er satt til Alle.
  
 **Gjør følgende for å løse dette problemet:**
  
 1. Tillat alle å se medlemmene av SharePoint gruppen.
  
 2. Fjern SharePoint-gruppen fra Til- eller Kopi-linjen i e-postmeldingen.
  
 3. Legg eksplisitt til brukerne i Til- eller Kopi-linjen hvis synligheten for medlemskap ikke kan endres for SharePoint gruppen.
  
Hvis du vil se flere detaljer, kan du se [HTTP Uautorisert til /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  