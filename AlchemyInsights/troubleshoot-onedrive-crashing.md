---
title: Feilsøke OneDrive-krasj
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749163"
---
# <a name="troubleshoot-onedrive-crashes"></a>Feilsøke OneDrive-krasj

Hvis OneDrive krasjer gjentatte ganger, kan du prøve disse feilsøkingstrinnene:

**Kontroller at registernøkler ikke er angitt:**

1. Bruk Registerredigering til å gå til HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Hvis DisableFileSyncNGSC finnes og satt til 1, åpner du nøkkelen og endrer verdien til 0.
3. Start OneDrive manuelt ved å gå til Start ![Trykk Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), skriv inn OneDrive i søkeboksen, og klikk deretter på OneDrive-skrivebordsappen.

**Tilbakestill OneDrive:**

Notater:

- Tilbakestilling av OneDrive kobler fra alle eksisterende synkroniseringstilkoblinger (inkludert din personlige OneDrive hvis konfigurert).
- Du vil ikke miste filer eller data ved å tilbakestille OneDrive på datamaskinen.

**Slik tilbakestiller du OneDrive:**

1. Åpne en Kjør-dialogboks ved å trykke Windows-tasten og R.
2. Skriv inn %localappdata%\Microsoft\OneDrive\onedrive.exe /reset, og trykk på OK. Et kommandovindu kan vises kort.
3. Start OneDrive manuelt ved å gå til Start ![Trykk Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), skriv inn OneDrive i søkeboksen, og klikk deretter på OneDrive-skrivebordsappen.

Notater:

- Hvis du hadde valgt å synkronisere bare noen mapper før tilbakestillingen, må du gjøre det igjen når synkroniseringen er fullført. Les [Velg hvilke OneDrive-mapper som skal synkroniseres med datamaskinen,](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   hvis du vil ha mer informasjon.
- Du må fullføre dette for din personlige OneDrive og OneDrive for Business.