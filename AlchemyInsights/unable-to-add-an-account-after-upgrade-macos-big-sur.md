---
title: Kan ikke legge til en konto etter oppgradering til macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506763"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Kan ikke legge til en konto etter oppgradering til macOS 11.6 Big Sur

Når du har oppgradert til macOS 11.6, kan det hende at OneDrive for jobb- eller skolekontoen eller den personlige OneDrive-kontoen din ikke vises i listen over kontoer, og du kan kanskje ikke logge på en annen konto fra appen.

En løsning er utviklet for dette problemet. Først må du finne ut om du kjører den frittstående versjonen eller Store av OneDrive:

- Velg OneDrive skyen på menylinjen > **Hjelp & Innstillinger**  >  **Innstillinger**  >  **Om**. Hvis versjonsnummeret ikke inkluderer **(frittstående),** har du appversjonen Store av produktet.

Hvis du bruker den frittstående versjonen av OneDrive, starter du maskinen på nytt og OneDrive automatiske oppdateringer til et bygg der dette problemet er løst. Hvis du vil installere bygget manuelt, kan du laste ned denne [.zip-filen,](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)pakke ut filen og kopiere OneDrive-appen til Programmer-mappen (ved å erstatte den eksisterende OneDrive-appen).

Hvis du bruker appversjonen Store, bør du vurdere å installere den frittstående versjonen av OneDrive. Denne versjonen fungerer på samme måte som App Store-versjonen, men gjør at Microsoft kan tilby oppdateringer raskere til brukere og koble dem til en versjon som inneholder løsningen på dette problemet.

1. Last ned den frittstående versjonen av [OneDrive som inneholder løsningen.](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)
2. Pakk ut filen, og kopier OneDrive-appen til Programmer-mappen (ved å erstatte den eksisterende OneDrive appen).

Hvis du trenger å bruke appversjonen Store, venter du på at appversjonen Store å lansere en versjon av appen som inneholder løsningen. Microsoft kan dessverre ikke formidle en estimert dato for en fast versjon som skal utgis fra app-Store.


