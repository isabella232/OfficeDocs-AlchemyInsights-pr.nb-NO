---
title: Problemer med å logge på Microsoft 365-apper
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
- "9000571"
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695188"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="52233-102">Løse Microsoft 365-appene data maskinens klarerte plattform modul fungerer ikke som den skal: melding</span><span class="sxs-lookup"><span data-stu-id="52233-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="52233-103">For å løse denne filen kan du prøve følgende:</span><span class="sxs-lookup"><span data-stu-id="52233-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="52233-104">Installer de nyeste oppdateringene for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) og [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="52233-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="52233-105">[Fjern Office-legitimasjon](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) ved hjelp av Windows-legitimasjons behandling.</span><span class="sxs-lookup"><span data-stu-id="52233-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="52233-106">**Obs!** Register banene for Office 2016 har blitt endret til 16,0.</span><span class="sxs-lookup"><span data-stu-id="52233-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="52233-107">(Eks: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="52233-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="52233-108">Prøv [bruker gjenopprettings prosessen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) for å løse problemer med klarert plattform modul (TPM).</span><span class="sxs-lookup"><span data-stu-id="52233-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="52233-109">Angi EnableADAL = 0 ved hjelp av følgende trinn:</span><span class="sxs-lookup"><span data-stu-id="52233-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="52233-110">Høyre klikk Start knappen i Windows, velg **Kjør**, Skriv inn **regedit**, og velg deretter **OK**.</span><span class="sxs-lookup"><span data-stu-id="52233-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="52233-111">Velg **Ja** for å tillate register redigering å gjøre endringer på enheten.</span><span class="sxs-lookup"><span data-stu-id="52233-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="52233-112">I register redigering legger du til en DWORD-verdi på **EnableADAL** med en innstilling på **0** under HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="52233-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="52233-113">Hvis du vil ha mer informasjon, kan du se [tilkoblings problemer i pålogging etter oppdatering til Office 2016 Bygg 16.0.7967 på Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="52233-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>