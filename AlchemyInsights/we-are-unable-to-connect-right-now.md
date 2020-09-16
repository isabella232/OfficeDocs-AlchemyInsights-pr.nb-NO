---
title: Aktiverings problem – vi kan ikke koble til akkurat nå
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725992"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Løse Microsoft 365-appene vi kan ikke koble til akkurat nå-meldingen

Hvis du får denne meldingen, kan du prøve følgende:

1. Kontroller brann muren, antivirus program varen og proxy-innstillingene for å bekrefte at de ikke blokkerer Internett-tilgang til Microsoft 365-apper. Se [Microsoft-URL-adresser og IP-adresseområder](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Gå til **Start**  >  -**kjøring**, og skriv deretter inn **Services. msc**. Kontroller at følgende tjenester kjører:
    - Automatisk konfigurasjon av Network tilkoblede enheter
    - Nettverks liste tjeneste
    - Nettverks plasserings forståelse
    - Hendelses Logg for Windows

Hvis en av disse tjenestene ikke kjører, kan du prøve å starte den. Hvis du har problemer med å starte tjenesten, kjører du følgende kommando ved å åpne en lede tekst med utvidede tillatelser:

**sfc/scannow**

Når denne kommandoen er ferdig, starter du data maskinen på nytt.

Hvis du vil ha mer informasjon, kan du se [«beklager, vi har ikke koblet deg til kontoen din. Prøv på nytt senere-feil når du aktiverer Office fra Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).