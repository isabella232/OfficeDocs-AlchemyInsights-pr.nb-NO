---
title: 932 oppgradere AADConnect
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
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806048"
---
# <a name="upgrade-azure-ad-connect"></a>Oppgradere Azure AD Connect

Som standard er automatisk oppgradering aktivert for Azure AD Connect, noe som bidrar til å sikre at du kjører den nyeste versjonen. Hvis du vil kontrollere innstillingene for automatisk oppgradering, kan du bruke **Get-ADSyncAutoUpgrade** -cmdleten i Azure ad PowerShell. Cmdleten returnerer én av følgende verdier:

- **Aktivert**: automatisk oppgradering er aktivert.

- **Deaktivert**: automatisk oppgradering er deaktivert.

- **Suspendert**: systemet er ikke lenger berettiget til å motta automatiske oppgraderinger. Du kan ikke konfigurere denne verdien. den er angitt av systemet.

Hvis du vil ha mer informasjon, kan du se [automatisk oppgradering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).

Hvis du vil laste ned den nyeste versjonen av Azure AD Connect, kan du gå til [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .
