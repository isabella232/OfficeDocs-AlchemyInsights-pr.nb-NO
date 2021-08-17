---
title: 932 Oppgradere AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9582f1f56e6730e35520b5d79bc245cd74bea0bf4db39b379a7cd133bafc16ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104821"
---
# <a name="upgrade-azure-ad-connect"></a>Oppgradere Azure AD Koble til

Automatisk oppgradering er som standard aktivert for Azure AD Koble til, noe som bidrar til å sikre at du kjører den nyeste versjonen. Hvis du vil bekrefte innstillingene for automatisk oppgradering, bruker du cmdleten **Get-ADSyncAutoUpgrade** i Azure AD PowerShell. Cmdleten returnerer én av følgende verdier:

- **Aktivert:** Automatisk oppgradering er aktivert.

- **Deaktivert:** Automatisk oppgradering er deaktivert.

- **Suspendert:** Systemet er ikke lenger kvalifisert til å motta automatiske oppgraderinger. Du kan ikke konfigurere denne verdien. den er angitt av systemet.

Hvis du vil ha mer informasjon, kan [du se Automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Hvis du vil laste ned den nyeste versjonen av Azure AD Koble til, går du til [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
