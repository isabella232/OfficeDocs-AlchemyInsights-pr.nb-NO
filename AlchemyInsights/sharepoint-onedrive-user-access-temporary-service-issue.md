---
title: Ytelses problemer – SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771253"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive langsomt, utilgjengelig eller ikke tilgjengelig for flere brukere

Hvis et OneDrive-eller SharePoint-nettsted ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et midlertidig tjeneste problem. [Kontroller instrument bordet for tjeneste tilstand](https://portal.office.com/adminportal/home#/servicehealth).

**Legge til og lisensiere brukeren**

Sikre at du [tilordner lisenser til brukere i Microsoft 365 for bedrifter](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Tilordne tillatelser**

Hvis brukeren er tilordnet en SharePoint-lisens og likevel mottar meldingen ingen tilgang, må du forsikre deg om at de har det [riktige tilgangs nivået](https://docs.microsoft.com/sharepoint/understanding-permission-levels) som er tilordnet.

**Vurder å bruke funksjonen for tilgangs forespørsel**

Med [tilgangs forespørsels funksjonen](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) kan personer be om tilgang til innhold som de ikke har tillatelse til å se.

**Tillat egen definert skript kan føre til problemer som nektes tilgang**

Det finnes visse scenarioer der funksjonen *Tillat egen definerte skript* kanskje presenterer en tilgang nektet. For en liste over funksjoner som påvirkes, sikkerhets hensyn og muligheten til å deaktivere funksjonen. Gå til [tillate eller ikke Tillat egen definert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

