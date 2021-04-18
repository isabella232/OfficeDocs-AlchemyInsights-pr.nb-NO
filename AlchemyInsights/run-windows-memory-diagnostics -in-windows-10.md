---
title: Kjøre Windows minnediagnose i Windows 10
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
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826676"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Kjøre Windows minnediagnose i Windows 10

Hvis Windows og apper på PC-en krasjer, fryser eller oppfører seg ustabilt, kan det hende du har et problem med PC-ens minne (RAM). Du kan kjøre Windows minnediagnose for å se etter problemer med PC-ens RAM.

Skriv inn **minnediagnose** i søkeboksen på oppgavelinjen, og velg deretter **Windows minnediagnose**. 

For å kjøre diagnosen må PC-en startes på nytt. Du har muligheten til å starte på nytt umiddelbart (lagre arbeidet, og lukk åpne dokumenter og e-postmeldinger først), eller planlegg at diagnosen skal kjøres automatisk neste gang PC-en startes på nytt:

![Windows minnediagnose](media/windows-memory-diagnostic.png)

Når PC-en startes på nytt, kjøres **Windows Diagnoseverktøy for minne** automatisk. Status og fremdrift vises mens diagnosen kjører, og du har muligheten til å avbryte diagnosen ved å trykke på **ESC**-knappen på tastaturet.

Når diagnosen er fullført, starter Windows normalt.
Rett etter du har startet på nytt, når skrivebordet vises, vises en varsling (ved siden av **Handlingssenter**-ikonet på oppgavelinjen), for å indikere om minnefeil ble funnet. Eksempel:

Her er Handlingssenter-ikonet: ![Handlingssenter-ikon](media/action-center-icon.png) 

Og en eksempelvarsling: ![Ingen minnefeil](media/no-memory-errors.png)

Hvis du gikk glipp av varslingen, kan du velge **Handlingssenter**-ikonet på oppgavelinjen, for å vise **Handlingssenter** og se en rullbar liste over varslinger.

Hvis du vil gå gjennom detaljert informasjon, skriver du inn **hendelse** i søkeboksen på oppgavelinjen, og velger deretter **Hendelsesliste**. Gå til **Windows-logger > System** i ruten til venstre i **Hendelsesliste**. Skann nedover listen i ruten til høyre, mens du ser på **Kilde**-kolonnen, til du ser hendelser med kildeverdien **Minnediagnose-resultater**. Uthev hver hendelse som dette, og se resultatinformasjonen i boksen under **Generell**-fanen under listen.
