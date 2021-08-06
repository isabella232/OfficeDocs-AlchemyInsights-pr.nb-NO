---
title: Tilordne grupper til Azure AD-rollen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036249"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Tilordne grupper til Azure AD-rollen

Hvis du vil tilordne en Azure AD-gruppe med kilde til autoritet i Azure AD til en Azure AD-rolle, utfører du følgende trinn:

1. Opprette en ny gruppe – Slik oppretter du en ny gruppe:

    a. Logg på administrasjonssenteret for Azure AD med **privilegerte rolleadministrator-** eller **globale administratortillatelser.**
    b. Velg **Azure Active Directory > Grupper > Alle grupper > Ny gruppe**.
    c. Opprett gruppen.

2. Tilordne rollen til gruppen enten under opprettelsen av gruppen eller etter at gruppen er opprettet.

    a. Hvis du vil tilordne en rolle til gruppen på tidspunktet da gruppen ble opprettet, kan du slå på veksleknappen **For Azure AD-roller** kan tilordnes gruppen og opprette gruppen.
    b. Hvis du vil tilordne en rolle til gruppen  etter at den er opprettet, går du til Tilordnede roller-fanen for den nyopprettede gruppen og tilordner rollen til gruppen.  

**Administrere medlemskap i en gruppe som er tilordnet Til Azure AD-rollen**

Hvis du vil hindre rettighetsutvidelse, kan bare privilegerte rolleadministratorer og globale administratorer endre medlemskapet i en gruppe som er tilordnet til en rolle. De kan imidlertid velge å tilordne en eier for en slik gruppe og delegere denne oppgaven.

Hvis du vil ha mer informasjon om hvordan du tilordner skygrupper til Azure AD-roller, kan du [se Tilordne en AD-roller til Skygruppe](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Hvis du vil ha mer informasjon om feilsøking av roller som er tilordnet til skygrupper, kan du se [Feilsøke roller som er tilordnet til skygrupper](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





