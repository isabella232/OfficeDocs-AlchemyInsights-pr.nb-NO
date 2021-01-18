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
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885392"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Tilordne grupper til Azure AD-rollen

Hvis du vil tilordne en Azure AD-gruppe med kilde til autoritet i Azure AD til en Azure AD-rolle, utfører du følgende trinn:

1. Opprette en ny gruppe – for å opprette en ny gruppe:

    a. Logg deg på administrasjons senteret for Azure AD med **privilegert rolle administrator** eller **globale administrator** tillatelser.
    b. Velg **Azure Active Directory > groups > alle grupper > ny gruppe**.
    c. Opprett gruppen.

2. Tilordne rollen til gruppen under opprettelse av grupper, eller etter at gruppen er opprettet.

    a. Hvis du vil tilordne en rolle til gruppen når du oppretter en gruppe, kan du bytte til Aktiver/deaktiver **Azure ad-roller for å tilordne gruppen** og opprette gruppen.
    b. Hvis du vil tilordne en rolle til gruppen etter at den er opprettet, går du til fanen **tilordnede roller** for den nylig opprettede gruppen og tilordner rollen til gruppen.  

**Behandle medlemskap i en gruppe som er tilordnet til Azure AD-rollen**

Som standard kan bare privilegerte rolle administratorer og globale administratorer endre medlemskapet for en gruppe som er tilordnet en rolle, for å hindre heving av tilgangs nivåer. De kan imidlertid velge å tilordne en eier for en slik gruppe og delegere denne oppgaven.

Hvis du vil ha mer informasjon om hvordan du tilordner Sky grupper til Azure AD-roller, kan du se [tilordne en annonse roller til Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). Hvis du vil ha mer informasjon om feil søking av roller som er tilordnet til Sky grupper, kan du se [Feilsøke roller tilordnet til Sky grupper](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





