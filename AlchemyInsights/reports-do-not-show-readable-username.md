---
title: Rapporter i Administrasjonssenter for Microsoft 365 viser ikke lesbart brukernavn
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: ff8eac6487ef544277c5ce2c0c0b7068c9d400ca
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2021
ms.locfileid: "59327823"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Rapporter i Administrasjonssenter for Microsoft 365 viser ikke lesbart brukernavn

Rapporter i Administrasjonssenter for Microsoft 365 viser ikke brukernavn, men viser i stedet alfanumeriske verdier, for eksempel B2BC6C15BB9FCDEA71E5CD302D228CC8.

Dette er forventet virkemåte og har blitt kommunisert i Meldingssenter (MC275344, publisert 3. august 2021). 

Globale administratorer kan tilbakestille denne endringen for leieren og vise identifiserbar brukerinformasjon hvis organisasjonens personvernpraksis tillater det. Slik tilbakestiller du endringen for leieren:

1. Gå til **Innstillinger** > **Organisasjonsinnstillinger** > [**Tjenester**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services ) i administrasjonssenteret, og velg **Rapporter**. 
1. Under **Velg hvordan du vil vise brukerinformasjon**, velger du **Vis identifiserbar brukerinformasjon i rapporter**, og deretter kjører du rapporten på nytt.