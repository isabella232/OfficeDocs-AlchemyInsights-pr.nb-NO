---
title: Reparer PST-filen før du importerer
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799105"
---
# <a name="repair-pst-file-before-importing"></a>Reparer PST-filen før du importerer

Før du importerer en PST-fil i Outlook, må du kontrollere at filen ikke er skadet ved å reparere filen:

1. Avslutt Outlook.

2. Finn og Kjør `Scanpst.exe` i Office program-mappen (c:\Programfiler (x86) \Microsoft Office\root\Office \<Version\> eller c:\Programfiler\Microsoft Office\root\Office \<Version\> ).

3. I **reparasjons verktøyet for innboks for Microsoft Outlook**klikker du **Bla gjennom** for å finne PST-filen (for eksempel i C:\Users \\<bruker navn \> \AppData\Local\Microsoft\Outlook). Velg PST-filen, og klikk deretter **Åpne**.

4. Klikk **Start** for å starte skanningen.

5. Hvis det blir funnet feil i filen, klikker du **Reparer**, og deretter klikker du **OK** når reparasjonen er fullført.

6. Prøv å importere PST-filen i Outlook på nytt.

Hvis du vil ha mer informasjon, kan du se [reparere Outlook-datafiler](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) og [løse problemer med import av en Outlook. PST-fil](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).
