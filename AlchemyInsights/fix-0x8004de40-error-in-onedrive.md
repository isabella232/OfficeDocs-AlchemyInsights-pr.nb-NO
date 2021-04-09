---
title: Løse 0x8004de40 i OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649757"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Løse 0x8004de40 i OneDrive

Hvis du kjører Windows 7 og får denne feilen, oppdaterer [du TLS 1.1 og TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard sikre protokoller i WinHTTP i Windows .

Hvis du kjører Windows 10, og du får en 0x8004de40 feilmelding med OneDrive:

- Start den berørte datamaskinen på nytt mens du er koblet til Acitve Directory-domenet.
- Hvis en omstart ikke løser problemet, kan du koble til og bli med på enheten på nytt fra Azure AD. 

**Obs!** Du bør være på bedriftsnettverket mens du utfører disse trinnene. Ikke utfør disse trinnene når du ikke er koblet til bedriftens infrastruktur (for eksempel når du er på reise). 

1. Åpne en forhøyet ledetekst ved å velge **Start**, høyreklikk **ledetekst**, og velg deretter Kjør som **administrator**.

1. Skriv *inn dsregcmd /leave, og* trykk **ENTER**.

1. Når du er ferdig, skriver du *inn dsregcmd /join og* trykker **ENTER.**

1. Lukk ledeteksten når du er ferdig.

1. Start datamaskinen på nytt, og logg på OneDrive.