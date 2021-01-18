---
title: SAML-deklarasjoner (tokener)
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885670"
---
# <a name="saml-assertions-tokens"></a>SAML-deklarasjoner (tokener)

1. Sikkerhets deklarasjoner Markup Language (SAML)-tokener er XML representasjoner av krav. Som standard er Windows Communication Foundation (WCF) som bruker i sikkerhets scenarioer i organisasjons nettverk utsteder koder. Hvis du vil ha mer informasjon, kan du se [SAML tokens og krav](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Microsoft Identity Platform sender ut flere typer sikkerhetstokener i behandlingen av hver godkjennings flyt. [Referansen for krav til SAML-token](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) beskriver formatet, sikkerhets egenskapene og innholdet i SAML 2,0-tokener.
3. Følg rettledningen i [konfigurerbare token-leve tid i Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) for å forstå hvordan du konfigurerer token-leve tid.
4. Følg Fremgangs måten i [denne artikkelen](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) for å forstå hvordan du konfigurerer Azure ad SAML token Encryption.
5. I Azure AD kan du konfigurere alternativer for sertifikat signering og algoritme for sertifikat signering. Hvis du vil ha mer informasjon, kan du se [Avanserte alternativer for sertifikat signering i SAML-token for Gallery-apper i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
