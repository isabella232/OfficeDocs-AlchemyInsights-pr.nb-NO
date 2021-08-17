---
title: Kan ikke aktivere Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: eb62dfce9f9507dd8806d91343cd39fe76e65594473683c1393d524f6c2d8a27
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893920"
---
# <a name="unable-to-activate-office"></a>Kan ikke aktivere Office

**Obs!** Hvis du bruker en eldre versjon av Windows (for eksempel Windows 7), må du kontrollere at TLS 1.2 er aktivert som standard. Hvis du vil ha mer informasjon, kan du se Oppdatere for å aktivere [TLS 1.1 og TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)som standard sikre protokoller i WinHTTP i Windows .

- Kontroller om abonnementet har utløpt.
- Kontroller at du har et abonnement som tillater klientlisenser, som for eksempel Office 365 Business eller Business Premium, og [kontroller at brukeren har en tilordnet lisens](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).
- Forsikre deg om at brukeren logger på Office med samme konto som lisensen er tildelt til.
- Sjekk [siden for Office 365-tjenestetilstand](https://docs.microsoft.com/office365/enterprise/view-service-health) for å se om det finnes kjente problemer med tjenesten.
- Kontroller brannmuren, antivirusprogramvaren og proxy-innstillingene for å bekrefte at de ikke blokkerer Microsoft 365-apper sin tilgang til internett. Se [URL-adresser og IP-adresseområder for Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL-adresser og IP-adresseområder for Office 365").

**Tips** På Windows-maskiner kan vi diagnostisere og ordne flere vanlige problemer med pålogging til Office for deg. Last ned og kjør **[assistent for støtte og gjenoppretting](https://aka.ms/SaRA-OfficeSignInScenario)** for å bruke vårt automatiserte verktøy.

Bruk følgende feilsøkingshandlinger:

- Åpne et Office-program og [logg av](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) eksisterende brukerkontoer. [Fjern](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) og [tilordne](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office-lisens på nytt, og deretter [logge på Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) ved hjelp av den berørte brukerkontoen.
- Kjør feilsøkingsverktøyet for [Aktivering](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Tilbakestill aktiveringsstatusen for Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Tilbakestill aktiveringsstatusen for Office")
- [Utfør en Tilkoblet reparasjon av Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Hvis du trenger ytterligere feilsøkingsløsninger, kan du se:  

- [Feil ved ulisensiert produkt og aktivering i Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [«Beklager, vi kan ikke koble til kontoen din. Prøv på nytt senere»-feil når du aktiverer Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)