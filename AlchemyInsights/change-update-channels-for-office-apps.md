---
title: Endre oppdateringskanaler for Office-apper
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440027"
---
# <a name="change-update-channels-for-office-apps"></a>Endre oppdateringskanaler for Office-apper

For nye Office-installasjoner bruker du nedlastingsinnstillinger for Office-programvare til å velge ønsket oppdateringskanal og deretter installere (eller installere) Office-apper på nytt. Hvis du vil ha mer informasjon, kan du se [Administrere innstillinger for nedlasting av programvare i Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Merk at** Oppdateringskanalen som er valgt ved hjelp av nedlastingsinnstillingene for Office-programvare, gjelder for alle brukere som utfører nye installasjoner ved hjelp av O365-portalen. Hvis du vil ha mer informasjon, kan du se [Laste ned og installere eller installere Microsoft 365 eller Office 2019 på nytt på en PC eller Mac](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

For eksisterende Office-installasjoner bruker du Office Deployment Tool (ODT) til å bytte til en annen oppdateringskanal:  

1. Last ned den nyeste versjonen av Office Deployment Tool (setup.exe) fra [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Identifiser navnet på kanalen du vil bytte til. Hvis du vil ha mer informasjon, kan du se [Konfigurasjonsalternativer for Office Deployment Tool](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Opprett en XML-fil for konfigurasjon som angir riktig kanalnavn, for eksempel update.xml.  
    a. <Configuration>  
    b. <oppdaterer **Channel="Månedlig"** />  
    c. </Configuration>
4. Fra en hevet ledetekst bytter du til mappeplasseringen der setup.exe ligger og kjører følgende kommando:  
    a. setup.exe /konfigurere update.xml
5. Start et Office-program (for eksempel **File**Excel), og velg deretter  >  **Filkonto**. Velg **Oppdateringsalternativer**for oppdatering nå i  >  **Update Now**Produktinformasjon-delen.

Hvis du vil ha mer informasjon, kan du se [Slik bytter du oppdateringskanaler for eksisterende Office-apper](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Hvis du vil bytte oppdateringskanaler for en valgt gruppe brukere eller ved hjelp av Configuration Manager (SCCM), kan du konfigurere innstillingen Oppdater kanal ved hjelp av Gruppepolicyobjektet. Hvis du vil ha mer informasjon, kan du se [Oversikt over oppdateringskanaler for Microsoft 365-apper](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Hvis du vil ha mer informasjon, kan du se [Administrere Office 365 ProPlus-kanaler for IT-kunder](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) og [administrere oppdateringer for Microsoft 365-apper med Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).