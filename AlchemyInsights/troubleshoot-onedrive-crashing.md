---
title: Feilsøke OneDrive krasj
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921016"
---
# <a name="troubleshoot-onedrive-crashes"></a>Feilsøke OneDrive krasj

Hvis OneDrive krasjer gjentatte ganger, kan du prøve disse feilsøkingstrinnene:

**Kontroller at registernøkler ikke er angitt:**

1. Ved hjelp av Registerredigering går du til HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Hvis DisableFileSyncNGSC finnes og er satt til 1, åpner du nøkkelen og endrer verdien til 0.
3. Starte OneDrive ved å gå til Start ![Trykk Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), skriv OneDrive i søkeboksen, og klikk deretter på OneDrive skrivebordsappen.

**Tilbakestill OneDrive:**

Merknader:

- Tilbakestilling OneDrive alle eksisterende synkroniseringstilkoblinger (inkludert personlige OneDrive hvis den er konfigurert).
- Du mister ikke filer eller data ved å tilbakestille OneDrive på datamaskinen.

**Slik tilbakestiller du OneDrive:**

1. Åpne en Kjør-dialogboks ved å trykke Windows og R.
2. Skriv inn %localappdata%\Microsoft\OneDrive\onedrive.exe /reset, og trykk OK. Et kommandovindu kan vises en kort stund.
3. Starte OneDrive ved å gå til Start ![Trykk Windows-tasten](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), skriv OneDrive i søkeboksen, og klikk deretter på OneDrive skrivebordsappen.

Merknader:

- Hvis du har valgt å synkronisere bare noen mapper før tilbakestillingen, må du gjøre dette på nytt når synkroniseringen er fullført. Les [Velge hvilke OneDrive mapper som skal synkroniseres til datamaskinen for](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)mer   informasjon.
- Du må fullføre dette for personlige OneDrive og OneDrive for Business.