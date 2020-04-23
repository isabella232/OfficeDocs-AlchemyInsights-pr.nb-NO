---
title: 932 Oppgradere AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766502"
---
# <a name="upgrade-azure-ad-connect"></a>Oppgrader Azure AD Connect

Som standard er automatisk oppgradering aktivert for Azure AD Connect, noe som bidrar til å sikre at du kjører den nyeste versjonen. Hvis du vil kontrollere de automatiske oppgraderingsinnstillingene, bruker du cmdleten **Get-ADSyncAutoUpgrade** i Azure AD PowerShell. Cmdleten returnerer én av følgende verdier:

- **Aktivert:** Automatisk oppgradering er aktivert.

- **Deaktivert:** Automatisk oppgradering er deaktivert.

- **Suspendert**: Systemet er ikke lenger kvalifisert til å motta automatiske oppgraderinger. Du kan ikke konfigurere denne verdien. det er satt av systemet.

Hvis du vil ha mer informasjon, kan du se [Automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Hvis du vil laste ned den nyeste [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)versjonen av Azure AD Connect, går du til .
