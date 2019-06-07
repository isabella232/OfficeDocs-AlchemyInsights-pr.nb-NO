---
title: Identifisere ekstern e-post videresending på postbokser i overvåkingslogger
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 518e4dd485ee7c54ce83e65794152e32f4c3a836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752025"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifisere når ekstern e-post videresending er konfigurert på postbokser

Når en bruker konfigurerer videresending av ekstern e-post på en postboks, er aktiviteten overvåket som en del av cmdleten **Set-postboks** . Du kan vise aktiviteten ved hjelp av sporing Logg Søk i Security-& overholdelsessenteret.

1. Logg på [Office 365 & kompatibilitet Sikkerhetssenter](https://protection.office.com/)

2. Klikk **Søk og undersøkelser** , og velg **Overvåk Logg Søk**.

3. Velg datointervallet i feltene **Startdato** og **Sluttdato** . Du trenger ikke å angi et brukernavn. Kontroller **aktiviteter** -feltet er satt til å **vise resultater for alle aktiviteter**.

4. Klikk **Søk**.

I resultatene klikker du **Filtreringsresultatene** og Skriv inn **Sett postboks** filterlisten for aktiviteten. Velg et kontrollregister i resultatene. I **Detaljer** -undermeny, klikker du **vil ha mer informasjon**. Du må se på detaljene for hver kontrollregister å finne ut om aktiviteten er knyttet til e-post videresending.

- **ObjectId**: alias verdien av postboksen som ble endret.

- **Parametere**: _ForwardingSmtpAddress_ angir måladressen for e-post.

- **Bruker-ID**: brukeren som konfigurert videresending av e-post på postboksen i **objekt-ID** -feltet.

Hvis du vil ha mer informasjon, kan du se [Determining som konfigurere e-post videresending for en bestemt postboks](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
