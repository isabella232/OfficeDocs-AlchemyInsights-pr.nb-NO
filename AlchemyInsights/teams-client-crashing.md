---
title: Krasjer Teams-klienten?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030679"
---
# <a name="teams-client-crashing"></a>Krasjer Teams-klienten?

Hvis Teams-klienten krasjer, kan du prøve følgende:

- Hvis du bruker Teams skrivebordsprogram, [forsikre deg om at appen er oppdatert til siste versjon](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Kontroller at alle [URL-adressene og adresseområdene til Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) er tilgjengelige.

- Logg på med administratorkontoen og kontroller [Tjenestetilstandsinstrumentbordet](https://docs.microsoft.com/office365/enterprise/view-service-health) for å bekrefte at ingen avbrudd eller tjenestereduksjon finnes.

 - Som et siste trinn kan du prøve å slette klientens hurtigbuffer for Teams:

    1.  Gå helt ut av skrivebordsklienten for Microsoft Teams. Du kan høyreklikke på **Teams** fra ikonstatusfeltet og klikke **Avslutt**eller Kjør oppgavebehandling og avslutt prosessen helt.

    2.  Gå til Filutforsker, og skriv inn %appdata%\Microsoft\teams.

    3.  Når du er i katalogen, ser du noen av følgende mapper:

         - Gå til **Appbuffer** under Hurtigbuffer, og slett filene i hurtigbufferen: %appdata%\Microsoft\teams\application cache\cache.

        - Slett alle filer i **Blob_lagring**: %appdata%\Microsoft\teams\blob_storage.

        - Slett alle filer i **Cache**: %appdata%\Microsoft\teams\Cache.

        - Slett alle filer i **databaser**: %appdata%\Microsoft\teams\databases.

        - Slett alle filer i **GUPUCache**: %appdata%\Microsoft\teams\GPUcache.

        - Slett alle filer i **IndeksertDB**: %appdata%\Microsoft\teams\IndexedDB.

        - Slett alle filer i **Lokal lagring**: %appdata%\Microsoft\teams\Local Storage.

        - Til slutt, slett alle filer i **tmp**: %appdata%\Microsoft\teams\tmp.

    4. Start Teams-klienten på nytt.
