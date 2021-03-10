---
title: Feilsøke problemer med SAML-signeringssertifikatet
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694444"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="c6a28-102">Feilsøke problemer med SAML-signeringssertifikatet</span><span class="sxs-lookup"><span data-stu-id="c6a28-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="c6a28-103">Utfør følgende anbefalte trinn for å løse problemet med SAML-signeringssertifikatet:</span><span class="sxs-lookup"><span data-stu-id="c6a28-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="c6a28-104">Når du legger til et virksomhetsprogram som støtter SSO, genererer Azure et sertifikat som kalles [SAML-signatursertifikatet.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)</span><span class="sxs-lookup"><span data-stu-id="c6a28-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="c6a28-105">Dette sertifikatet har en utløpsdato på tre år.</span><span class="sxs-lookup"><span data-stu-id="c6a28-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="c6a28-106">Hvis du vil endre utløpsdatoen for sertifikatet, kan du se Tilpasse utløpsdatoen for forbundssertifikatet og rulle [den over til et nytt sertifikat.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)</span><span class="sxs-lookup"><span data-stu-id="c6a28-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="c6a28-107">Azure bruker dette sertifikatet til å signere SAML-tokenene som er forespurt av programmet, og sender det over til programmet for å få en vellykket SSO.</span><span class="sxs-lookup"><span data-stu-id="c6a28-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="c6a28-108">For at dette skal fullføres må du laste ned sertifikatet fra Azure Portal og sende det til programleverandøren for å fullføre SSO-prosessen.</span><span class="sxs-lookup"><span data-stu-id="c6a28-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="c6a28-109">Når denne prosessen er fullført, vil programmet klarere dette sertifikatet, og alle SAML-tokener som er signert med dette sertifikatet, godkjennes av programmet.</span><span class="sxs-lookup"><span data-stu-id="c6a28-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="c6a28-110">Hvis dette sertifikatet utløper, oppretter du et nytt sertifikat, oppdaterer det til programleverandøren og gjør det aktivt på Azure-siden.</span><span class="sxs-lookup"><span data-stu-id="c6a28-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="c6a28-111">Hvis du vil ha mer informasjon, kan du se Fornye et [sertifikat som snart utløper.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)</span><span class="sxs-lookup"><span data-stu-id="c6a28-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="c6a28-112">Hvis sertifikatet utløper, blokkeres ikke brukeren.</span><span class="sxs-lookup"><span data-stu-id="c6a28-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="c6a28-113">[Legg til en e-postadresse for](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) varsler som skal mottas før det gjeldende sertifikatet utløper.</span><span class="sxs-lookup"><span data-stu-id="c6a28-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="c6a28-114">Trinn 4 er valgfritt.</span><span class="sxs-lookup"><span data-stu-id="c6a28-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="c6a28-115">Endre alternativene for SAML-sertifikatsignering i et program og algoritmen for sertifikatsignering.</span><span class="sxs-lookup"><span data-stu-id="c6a28-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="c6a28-116">Hvis du vil ha mer informasjon, kan du se Endre alternativer for [sertifikatsignering og signeringsalgoritme.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="c6a28-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

