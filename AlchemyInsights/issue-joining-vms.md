---
title: Problem med å bli med i VM-er
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: nb-NO
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885667"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="5b11a-102">Problem med å bli med i VM-er</span><span class="sxs-lookup"><span data-stu-id="5b11a-102">Issue joining VMs</span></span>

<span data-ttu-id="5b11a-103">Hvis du vil løse problemer som oppstår mens du prøver å koble til VM-er, utfører du følgende trinn:</span><span class="sxs-lookup"><span data-stu-id="5b11a-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="5b11a-104">Prøv å logge på med **UPN** -formatet (for eksempel «joeuser@contoso.com») i stedet for **sAMAccountName** -formatet (CONTOSO\joeuser).</span><span class="sxs-lookup"><span data-stu-id="5b11a-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="5b11a-105">Kontroller at du har aktivert passord synkronisering i henhold til trinnene som er beskrevet i *komme i gang* -veiledningen.</span><span class="sxs-lookup"><span data-stu-id="5b11a-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="5b11a-106">Kontroller at den berørte bruker kontoen ikke er en ekstern konto i Azure AD-leieren.</span><span class="sxs-lookup"><span data-stu-id="5b11a-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="5b11a-107">Eksterne brukere kan ikke logge seg på det forvaltede domenet fordi Azure AD Domain Services ikke har legitimasjon for slike bruker kontoer.</span><span class="sxs-lookup"><span data-stu-id="5b11a-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="5b11a-108">Hvis den berørte bruker kontoen er en bruker konto som bare er en sky, må du sørge for at brukere har endret passordet sitt etter at du aktiverte Azure AD Domain Services.</span><span class="sxs-lookup"><span data-stu-id="5b11a-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="5b11a-109">Dette trinnet fører til at legitimasjons nummer som kreves for Azure AD Domain Services, genereres.</span><span class="sxs-lookup"><span data-stu-id="5b11a-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="5b11a-110">Hvis de berørte bruker kontoene synkroniseres fra en lokal katalog, må du kontrollere at den anbefalte utgivelsen av Azure AD Connect er konfigurert til å utføre en fullstendig synkronisering.</span><span class="sxs-lookup"><span data-stu-id="5b11a-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="5b11a-111">Hvis problemet vedvarer etter at du har bekreftet trinn 4, utfører du følgende kommandoer fra synkroniserings maskinen:</span><span class="sxs-lookup"><span data-stu-id="5b11a-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="5b11a-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="5b11a-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>