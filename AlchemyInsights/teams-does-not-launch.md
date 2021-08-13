---
title: Teams starter ikke
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813353"
---
# <a name="teams-doesnt-launch"></a>Teams starter ikke

Hvis du prøver å åpne Microsoft Teams, men den aldri starter, kan du prøve følgende:

1. Bla til **%appdata%\Microsoft\Teams**.
1. Slett innholdet i mappen.
1. Start datamaskinen på nytt, og prøv å starte Teams.

Du må kanskje installere Teams. Slik installerer du på nytt:

1. Avinstaller Teams ved hjelp av Kontrollpanel.
1. Bla til **%appdata%\Microsoft\Teams\Application Cache**.
1. Slett innholdet i mappen.
1. Bla til **%appdata%\Microsoft\teams\Cache**.
1. Slett innholdet i mappen.
1. Start datamaskinen på nytt, og last deretter ned og installer Teams.

Hvis du vil kjøre en diagnose på leieren for en bestemt bruker som ikke kan logge på, starter du et nytt søk med nøkkelordet **TeamsUserUnableToSignIn** og følger instruksjonene.