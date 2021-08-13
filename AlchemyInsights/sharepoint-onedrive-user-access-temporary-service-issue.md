---
title: Ytelsesproblemer– SharePoint eller OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093770"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint eller OneDrive Langsom, Utilgjengelig eller Utilgjengelig for flere brukere

Hvis et OneDrive eller SharePoint nettstedet ikke er tilgjengelig for flere brukere som tidligere hadde tilgang, kan det være et midlertidig tjenesteproblem. [Kontroller instrumentbordet for tjenestetilstand](https://portal.office.com/adminportal/home#/servicehealth).

**Legge til og lisensiere brukeren**

Kontroller at du [tilordner lisenser til brukere i Microsoft 365 for bedrifter](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Tilordne tillatelser**

Hvis brukeren har blitt tilordnet en Sharepoint-lisens og fremdeles mottar en melding om at det ikke er tilgang, må du kontrollere at de har riktig [tilgangsnivå](https://docs.microsoft.com/sharepoint/understanding-permission-levels) tilordnet.

**Vurder å bruke funksjonen for tilgangsforespørsel**

Funksjonen [for tilgangsforespørsler](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) gjør det mulig for personer å be om tilgang til innhold som de for øyeblikket ikke har tillatelse til å se.

**Tillat egendefinert skript kan føre til problemer med tilgang som ikke er tilgjengelig**

Det finnes visse scenarier der tillat *egendefinert skript-funksjonen* kan presentere en ingen tilgang. For en liste over funksjoner som er berørt, sikkerhetshensyn og muligheten til å deaktivere funksjonen. Gå til [Tillat eller hindre egendefinert skript](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

