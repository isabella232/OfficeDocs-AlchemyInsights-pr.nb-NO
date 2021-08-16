---
title: Intune Device Inventory
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014081"
---
# <a name="intune-device-inventory"></a>Intune Device Inventory

Enheter-bladet gir administratoren innsikt i enheter som er under administrasjon i Intune per enhet. Informasjonen som vises, omfatter: Maskinvare, oppdagede programmer, tilstand for enhetssamsvar og tilstanden For enhetskonfigurasjon.

Lagerdata for maskinvare og oppdagede programmer samles inn i en sjudagers syklus. Programmene og bestemte elementer av maskinvare som rapporteres, varierer avhengig av operativsystemet på enheten og om enheten er personlig eller bedriftseid.

Hvis du vil ha mer informasjon, [kan du se Se enhetsdetaljer i Intune](https://docs.microsoft.com/intune/device-inventory).

**SPØRSMÅL OG SVAR**

Spørsmål: Jeg mottar ikke en fullstendig liste over programmer som finnes på Intune-registrerte Windows enheter. hvorfor ikke?

A: Foreløpig er bare moderne apper oppført for Windows 10 PC-er som identifiseres som bedriftsenheter. Intune samler ikke inn informasjon om Win32-apper som er installert på disse enhetene.

Spørsmål: Hvorfor samles ikke telefonnumre inn fra alle enheter?

A: Telefoner som er kategorisert som bedriftsenheter i Intune, identifiseres ikke med hele telefonnummeret sitt når du for eksempel kjører en lagerrapport for mobilenheter. Telefonnumre for bring-you-own-device er alltid delvis maskert med stjerner (****), og viser bare de siste fire sifrene.