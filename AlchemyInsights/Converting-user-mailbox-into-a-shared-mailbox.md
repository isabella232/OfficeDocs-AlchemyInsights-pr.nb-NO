---
title: Konverterer brukerens postboks til en delt postboks?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2019
ms.locfileid: "28303563"
---
Du kan bare konvertere en Brukerpostboks til en delt postboks Hvis brukeren har en lisens for Exchange. Når postboksen er konvertert, vil den fortsette å vises i brukerlisten over aktive fordi listen inneholder delte postbokser. Imidlertid vil konverterte postboksen også vises i listen over delte postbokser. 
  
Hvis du prøver å konvertere en postboks i Exchange Administrator-konsollen, og konverteringen mislykkes, tømme hurtigbufferen og informasjonskapslene, og prøv på nytt. Hvis det fortsatt ikke fungerer, kan du prøve å konvertere postboks i Exchange Management Shell ved å kjøre følgende kommando:
  
```
Set-Mailbox -Type Shared
```

Mer informasjon om konvertering av postboksen er tilgjengelig i [konvertere en Brukerpostboks til en delt postboks](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).
  
