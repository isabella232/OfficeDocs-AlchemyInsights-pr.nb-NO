---
title: Konfigurere tjenestetilkoblingspunkt (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036147"
---
# <a name="configure-service-connection-point-scp"></a>Konfigurere tjenestetilkoblingspunkt (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Årsak:** Kan ikke lese SCP-objektet og få informasjon om Azure AD-leieren
- **Løsning:** Se delen Konfigurere [et tjenestetilkoblingspunkt](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Handlingsplan**

- Kontroller om enheten har mottatt gruppepolicyobjektet for den kontrollerte valideringen.
- Kontroller at gruppepolicyobjektet har opprettet registernøklene.
- Kontroller at du har to nøkler opprettet med katalog-ID-en og onmicrosoft-domenet.

**Konfigurere registerinnstilling for klientsiden for SCP**

Bruk følgende eksempel til å opprette et gruppepolicyobjekt (GPO) til å distribuere en registerinnstilling som konfigurerer en SCP-oppføring i registeret på enhetene.

1. Åpne en konsoll for gruppepolicybehandling, og opprett et nytt gruppepolicyobjekt i domenet.
     - Gi det nyopprettede gruppepolicyobjektet et navn (for eksempel ClientSideSCP)

2. Rediger gruppepolicyobjektet, og finn følgende bane: Datamaskinkonfigurasjon > **Innstillinger > Windows-innstillinger > registeret**.

3. Høyreklikk **registeret, og** velg **Nytt > registerelement**.

4. Konfigurer følgende **på** Generelt-fanen:
  
- **Handling:** Oppdater
    
- **Struktur:** HKEY_LOCAL_MACHINE
    
- **Nøkkelbane:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Verdinavn:** TenantId
    
- **Verditype**: REG_SZ
    
- **Verdidata:** GUID- eller katalog-ID-en for Azure AD-forekomsten (Denne verdien finnes i **Azure Portal > Azure Active Directory > Egenskaper > Katalog-ID**)
 
- Klikk **OK**.
 
5. Høyreklikk **registeret, og** velg **Nytt > registerelement**.

6. Konfigurer følgende **på** Generelt-fanen:
  
- **Handling:** Oppdater
    
- **Struktur:** HKEY_LOCAL_MACHINE
    
- **Nøkkelbane:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Verdinavn:** TenantName
    
- **Verditype**: REG_SZ
    
- **Verdidata:** Det bekreftede domenenavnet hvis du bruker et forbundsmiljø, for eksempel AD FS. Det bekreftede domenenavnet eller onmicrosoft.com domenenavnet (for eksempel contoso.onmicrosoft).com hvis du bruker administrert miljø

- Klikk **OK**.

7. Lukk redigeringsprogrammet for det nylig opprettede gruppepolicyobjektet.

8. Koble det nylig opprettede gruppepolicyobjektet til den ønskede organisasjonsenheten som inneholder domenekretserte datamaskiner som tilhører den kontrollerte utrullingspopulasjonen.

Hvis du vil ha mer informasjon, kan du se [Kontrollert validering av hybrid Azure AD-sammenføyning – Azure AD | Microsoft Docs og](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)  [Feilsøking av hybrid Azure Active Directory-sammenføyde enheter | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









