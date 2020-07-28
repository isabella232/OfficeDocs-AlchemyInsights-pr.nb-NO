---
title: Apple MDM Push Sertifikat er ikke satt opp
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
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440004"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="fcfb3-102">Apple MDM Push Sertifikat er ikke satt opp</span><span class="sxs-lookup"><span data-stu-id="fcfb3-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="fcfb3-103">Et Apple MDM Push Certificate (også kjent som et APPLE Push Notification Service(APNS)-sertifikat) er ikke konfigurert for abonnementet.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="fcfb3-104">Uten et Apple MDM Push Sertifikat konfigurert, kan du ikke registrere og administrere iOS- og Mac OS-enheter.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="fcfb3-105">Når du har lagt til sertifikatet i Intune, kan brukere installere Firmaportal-appen for å registrere iOS-enhetene sine.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="fcfb3-106">Velg **"Jeg godtar."**</span><span class="sxs-lookup"><span data-stu-id="fcfb3-106">Select **"I agree."**</span></span> <span data-ttu-id="fcfb3-107">for å gi Microsoft tillatelse til å sende data til Apple.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="fcfb3-108">Velg **Last ned csr** intune sertifikatsigneringsforespørselen som kreves for å opprette et Apple MDM push-sertifikat.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="fcfb3-109">Filen brukes til å be om et klareringsrelasjonssertifikat fra Apple Push Certificates Portal.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="fcfb3-110">Velg **Opprett MDM push-sertifikatet** for å gå til Apple Push Certificates Portal.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="fcfb3-111">Logg på med Apple ID-en for firmaet, og velg deretter **Opprett et sertifikat**.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="fcfb3-112">Velg **Velg fil**, bla til forespørselsfilen for sertifikatsignering, og velg deretter Last **opp**.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="fcfb3-113">Velg **Last ned** på Bekreftelse-siden for å laste ned sertifikatfilen (PEM), og lagre filen lokalt.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="fcfb3-114">**Merk:** Sertifikatet er knyttet til Apple ID-en som brukes til å opprette det.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="fcfb3-115">Som en beste praksis, bruk en Apple ID for å administrere oppgaver, og kontroller at postboksen overvåkes av mer enn én person eller ved hjelp av en distribusjonsliste.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="fcfb3-116">Bruk aldri en personlig Apple-ID.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="fcfb3-117">Bruk samme Apple ID til å fornye Apple Push-sertifikatet hver 12.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="fcfb3-118">Skriv inn Apple ID-en som brukes til å opprette Apple MDM push-sertifikatet ditt.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="fcfb3-119">Registrer denne ID-en som en påminnelse for når du trenger å fornye sertifikatet.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="fcfb3-120">Gå til sertifikatfilen (PEM), velg **Åpne**, og velg deretter **Last opp**.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="fcfb3-121">Med push-sertifikatet kan Intune registrere og administrere Apple-enheter.</span><span class="sxs-lookup"><span data-stu-id="fcfb3-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>