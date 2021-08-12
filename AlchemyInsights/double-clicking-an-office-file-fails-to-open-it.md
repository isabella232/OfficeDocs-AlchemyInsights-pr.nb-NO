---
title: Når du dobbeltklikker en Office filen, åpnes den ikke
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 519051ac0ffc11d2b17c14959464c1123654bef38d6e10efd252b4ff3d8bbc1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965110"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a>Når du dobbeltklikker en Office filen, åpnes den ikke

Når du har dobbeltklikket Office en fil, kan det hende du ser at programmet er åpent, men selve filen åpnes ikke. Eller du kan få feilmeldingen: «Det oppstod et problem under sending av kommandoen til programmet.» Det finnes mange årsaker til dette, men de to vanligste løsningene er:

- I Excel må du kontrollere at DDE-alternativet ikke er avmerket. Du finner alternativet ved å opprette en ny arbeidsbok og deretter velge Fil > **Alternativer > Avansert**. Fjern **merket** for Ignorer andre programmer som bruker dynamiske data Exchange **(DDE) under Generelt.**

- Kjør en tilkoblet reparasjon for å gjenopprette standardinnstillingene. Klikk på Windows Start-knappen, og søk etter «Kontrollpanel». Åpne Kontrollpanel **, og** gå til Programmer > Programmer **og funksjoner**. Høyreklikk deretter på Microsoft Office **[Versjon]** og velg **Endre > tilkoblet reparasjon**.

Hvis ingen av disse løsningene fungerer, finner du en mer fullstendig liste over løsninger i støtteartikkelen. [Dobbeltklikking](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)av en Office fil kan ikke åpne den .
