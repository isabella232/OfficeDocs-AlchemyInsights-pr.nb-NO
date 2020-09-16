---
title: Feilsøke OneDrive-krasj
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665007"
---
# <a name="troubleshoot-onedrive-crashes"></a>Feilsøke OneDrive-krasj

Hvis OneDrive krasjer gjentatte ganger, kan du prøve disse feil søkings trinnene:

**Kontroller at Register nøkler ikke er angitt:**

1. Bruk register redigering til å gå til HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Hvis DisableFileSyncNGSC finnes og satt til 1, åpner du nøkkelen og endrer verdien til 0.
3. Start OneDrive manuelt ved å gå til Start ![Trykk Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), Skriv inn OneDrive i søke boksen, og klikk deretter på skrive bords programmet OneDrive.

**Tilbakestill OneDrive:**

Merknader

- Hvis du tilbakestiller OneDrive, kobles alle de eksisterende synkroniserings tilkoblingene fra (inkludert din personlige OneDrive hvis den er konfigurert).
- Du mister ikke filer eller data ved å tilbakestille OneDrive på data maskinen.

**Slik tilbakestiller du OneDrive:**

1. Åpne en Kjør-dialogboks ved å trykke Windows-tasten og R.
2. Skriv inn% localappdata% \Microsoft\OneDrive\onedrive.exe/reset, og trykk OK. Et kommando vindu kan vises kort.
3. Start OneDrive manuelt ved å gå til Start ![Trykk Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), Skriv inn OneDrive i søke boksen, og klikk deretter på skrive bords programmet OneDrive.

Merknader

- Hvis du har valgt å synkronisere bare enkelte mapper før du tilbakestiller, må du gjøre det på nytt når synkroniseringen er fullført. Les [velge hvilke OneDrive-mapper som skal synkroniseres til data maskinen](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   for mer informasjon.
- Du må fullføre dette for din personlige OneDrive og OneDrive for Business.