---
title: EWS マネージ API の再配布の要件
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: EWS マネージ API アセンブリをアプリケーションと共に再配布する方法を紹介します。
ms.openlocfilehash: d8fc57c4a2b3ed7d6218aeeed0fe88c2d3e0fbe0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759178"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a><span data-ttu-id="5da3d-103">EWS マネージ API の再配布の要件</span><span class="sxs-lookup"><span data-stu-id="5da3d-103">Redistribution requirements for the EWS Managed API</span></span>

<span data-ttu-id="5da3d-104">EWS マネージ API アセンブリをアプリケーションと共に再配布する方法を紹介します。</span><span class="sxs-lookup"><span data-stu-id="5da3d-104">Find out how you can redistribute the EWS Managed API assemblies with your application.</span></span>
  
<span data-ttu-id="5da3d-105">EWS のマネージ API アプリケーションを設計する際もたい方法、ユーザーにリリースするが検討してください。</span><span class="sxs-lookup"><span data-stu-id="5da3d-105">As you design your EWS Managed API application, you'll also want to consider how you will release it to your users.</span></span> 
  
## <a name="redistributing-your-ews-managed-api-application"></a><span data-ttu-id="5da3d-106">EWS マネージ API アプリケーションの再配布</span><span class="sxs-lookup"><span data-stu-id="5da3d-106">Redistributing your EWS Managed API application</span></span>

<span data-ttu-id="5da3d-p101">アプリケーションが Exchange サーバー上に配置されている場合を除き、EWS マネージ API アセンブリを再配布する必要があります。EWS マネージ API のダウンロードには、再配布できる次の 2 つのアセンブリが含まれています。Microsoft.Exchange.WebServices.dll と Microsoft.Exchange.WebServices.Auth.dll。EWS マネージ API アプリケーションをリリースする方法を設計する際に、次の情報を考慮してください。</span><span class="sxs-lookup"><span data-stu-id="5da3d-p101">Unless your application is located on the Exchange server, you will need to redistribute the EWS Managed API assemblies. The EWS Managed API download contains two assemblies that you can redistribute: Microsoft.Exchange.WebServices.dll and Microsoft.Exchange.WebServices.Auth.dll. Keep the following information in mind when you design how you will release your EWS Managed API application:</span></span>
  
- <span data-ttu-id="5da3d-p102">EWS マネージ API は、ダウンロードして、Exchange サーバーを対象とするアプリケーションと共に配布できるように設計されています。また、アプリケーションで EWS マネージ API をダウンロードすることもできます。</span><span class="sxs-lookup"><span data-stu-id="5da3d-p102">The EWS Managed API was designed such that you can download it and distribute it with your application that targets an Exchange server. Alternatively, your application can download the EWS Managed API.</span></span>
    
- <span data-ttu-id="5da3d-112">EWS マネージ API を使用して、Exchange Online、Office 365 の一部としての Exchange Online、または Exchange Server 2007 以降のオンプレミス バージョンの Exchange と通信することができます。</span><span class="sxs-lookup"><span data-stu-id="5da3d-112">You can use the EWS Managed API to communicate with an Exchange server running Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange Server 2007.</span></span>
    
- <span data-ttu-id="5da3d-p103">バージョン 2.1 以降のバージョンの EWS マネージ API で、グローバル アセンブリ キャッシュ (GAC) に API をインストールできます。MSI は自動的に DLL を GAC に追加し、ユーザーごとではなく、コンピューターごとにアクセス可能である。</span><span class="sxs-lookup"><span data-stu-id="5da3d-p103">In versions of the EWS Managed API starting with version 2.1, you can install the API in the Global Assembly Cache (GAC). The MSI will automatically add the DLL to the GAC and will be accessible on per computer basis, not on a per user basis.</span></span>
    
<span data-ttu-id="5da3d-p104">ライセンス条項は EWS マネージ API のダウンロードに含まれています。EWS マネージ API で実行できる作業に関する認証情報の条項について確認してください。</span><span class="sxs-lookup"><span data-stu-id="5da3d-p104">The license terms are included in the EWS Managed API download. Review the terms for the authoritative information about what you can do with the EWS Managed API.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="5da3d-117">関連項目</span><span class="sxs-lookup"><span data-stu-id="5da3d-117">See also</span></span>


- [<span data-ttu-id="5da3d-118">Exchange の EWS クライアントの設計の概要</span><span class="sxs-lookup"><span data-stu-id="5da3d-118">EWS client design overview for Exchange</span></span>](ews-client-design-overview-for-exchange.md)
    
- [<span data-ttu-id="5da3d-119">EWS マネージ API (ダウンロード)</span><span class="sxs-lookup"><span data-stu-id="5da3d-119">EWS Managed API (download)</span></span>](http://aka.ms/ews-managed-api-readme)
    

