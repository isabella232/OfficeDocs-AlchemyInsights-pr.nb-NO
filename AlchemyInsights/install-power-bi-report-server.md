---
title: Installere Power BI-rapportserveren
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1304"
- "2500001"
ms.openlocfilehash: 3ea596547093773ab872ca34e8dd3a4e49e59fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755104"
---
# <a name="install-power-bi-report-server"></a>Installere Power BI-rapportserveren

1. Finn plasseringen til PowerBIReportServer.exe, og start installasjons programmet.

2. Velg **Installer Power bi-rapportserver**.

3. Velg en utgave som skal installeres, og velg deretter **neste**.

4. Du kan velge enten evaluering eller utvikler-utgave fra rulle gardin listen.  Ellers kan du skrive inn en produkt nøkkel for serveren du har fått fra enten Power BI-tjenesten eller volum lisens tjeneste senteret. Hvis du vil ha mer informasjon om hvordan du får tak i produkt nøkkelen, kan du se delen før du begynner. Les og godta lisens vilkårene og betingelsene, og velg deretter **neste**.

5. Du må ha en database motor tilgjengelig for å lagre rapportserver-databasen. Velg **neste** for å installere bare rapportserveren.

6. Angi installasjons plasseringen for rapportserveren. Velg **Installer** for å fortsette.

7. Etter et vellykket oppsett velger du **Konfigurer rapportserver** for å starte Reporting Services Configuration Manager.

Du trenger ikke en SQL Server-database motor-server tilgjengelig på installasjons tidspunktet. Du trenger en for å konfigurere Reporting Services etter installasjon.

Hvis du vil ha mer informasjon: https://docs.microsoft.com/power-bi/report-server/install-report-server
