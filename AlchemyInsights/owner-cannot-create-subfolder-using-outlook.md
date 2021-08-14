---
title: Eieren kan ikke opprette undermappe ved hjelp av Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063133"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Eieren kan ikke opprette undermappe ved hjelp av Outlook

**Det er et pågående problem med eiere av fellesmapper som oppretter undermapper ved hjelp av Outlook. Problemet blir løst snart.**

I mellomtiden kan du bruke en av følgende midlertidige løsninger:

1. Bruk Outlook for MAC til å opprette undermappen fordi problemet bare påvirker Outlook for skrivebordsvinduer (alle versjoner)
2. Få administrator til å opprette undermappen ved hjelp av EXO Shell eller EAC
3. Endre DefaultPublicFolderMailbox/EffectivePublicFolderMailbox for brukeren til en annen postboks enn innholdspostboksen for mappen som forårsaker problemet  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Vent en time, start Outlook-klienten på nytt