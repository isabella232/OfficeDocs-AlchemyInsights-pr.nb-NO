---
title: Fjerne bakgrunnstjenesten for Microsoft Search i Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816333"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>Fjerne bakgrunnstjenesten for Microsoft Search i Bing

Hvis du vil fjerne bakgrunnstjenesten for Microsoft Search i Bing, kan du prøve følgende løsninger:

1. Hvis du vil gå tilbake til de opprinnelige innstillingene for søkemotoren, gjør du følgende:

    a. Bytt **av veksleknappen Bruk [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Bing som standard søkemotor**.

    b. [Gå til administrasjonssenteret for Microsoft 365,](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) og fjern innstillingen som påvirker alle brukerne i organisasjonen.

2. Hvis du vil fjerne bakgrunnstjenesten fra en enkelt enhet, gjør du følgende oppgaver:

    a. Velg **Kontrollpanel > programmer > programmer og funksjoner**.

    b. Høyreklikk Microsoft **Søk i Bing** under listen over installerte programmer, og klikk deretter **Avinstaller**.

3. Hvis du vil fjerne bakgrunnstjenesten fra flere enheter i organisasjonen, logger du på som administrator og kjører følgende kommando i et skript: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
