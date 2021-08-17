---
title: SAML-påstander (tokener)
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
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109249"
---
# <a name="saml-assertions-tokens"></a>SAML-påstander (tokener)

1. SAML-tokener (Security Assertions Markup Language) er XML-fremstillinger av krav. Som standard utstedes SAML-tokener Windows Communication Foundation (WCF) i sikkerhetsscenarioer i forbund. Hvis du vil ha mer informasjon, [kan du se SAML-tokener og krav](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).
2. Den Microsofts identitetsplattform sender ut flere typer sikkerhetstokener i behandlingen av hver godkjenningsflyt. [REFERANSE for SAML-tokenkrav](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) beskriver formatet, sikkerhetsegenskapene og innholdet i SAML 2.0-tokener.
3. Følg veiledningen i Konfigurerbar levetid for [token i](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) Microsofts identitetsplattform å forstå hvordan du konfigurerer levetid for tokener.
4. Følg fremgangsmåten i denne artikkelen [for](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) å forstå hvordan du konfigurerer Azure AD SAML-tokenkryptering.
5. I Azure AD kan du konfigurere alternativer for sertifikatsignering og algoritmen for sertifikatsignering. Hvis du vil ha mer informasjon, kan du se [Avanserte alternativer for sertifikatsignering i SAML-tokenet for galleriapper i Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).
