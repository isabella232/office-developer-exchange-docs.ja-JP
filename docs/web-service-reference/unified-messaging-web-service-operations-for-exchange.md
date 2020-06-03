---
title: Exchange のユニファイドメッセージング web サービスの操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Unified
api_type:
- schema
ms.assetid: d92455bd-24e8-4255-9f93-2bdeff00d42d
description: Exchange でのユニファイドメッセージング web サービスの操作に関する参照情報を検索します。
ms.openlocfilehash: b13ca2fbc44846db0bc98b3961916ba5d0872310
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529715"
---
# <a name="unified-messaging-web-service-operations-for-exchange"></a><span data-ttu-id="2bb01-103">Exchange のユニファイドメッセージング web サービスの操作</span><span class="sxs-lookup"><span data-stu-id="2bb01-103">Unified Messaging web service operations for Exchange</span></span>

<span data-ttu-id="2bb01-104">Exchange でのユニファイドメッセージング web サービスの操作に関する参照情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="2bb01-104">Find reference information for the Unified Messaging web service operations in Exchange.</span></span>
  
<span data-ttu-id="2bb01-105">ユニファイドメッセージング web サービスは、クライアントアプリケーションが、ユニファイドメッセージングのプロパティの読み取りおよび変更、ボイスメールメッセージの再生、案内応答の再生、およびテレフォニーデバイスを介したメールボックスアイテムのディクテーションを行えるようにする多くの操作を提供します。</span><span class="sxs-lookup"><span data-stu-id="2bb01-105">The Unified Messaging web service provides many operations that enable client applications to read and change Unified Messaging properties, play voice mail messages, record greetings, and dictate mailbox items over telephony devices.</span></span> <span data-ttu-id="2bb01-106">このセクションの記事では、要求の全体的な構造と、操作に対する応答メッセージについて説明します。</span><span class="sxs-lookup"><span data-stu-id="2bb01-106">The articles in this section provide information about the overall structure of the request and response messages for the operations.</span></span> <span data-ttu-id="2bb01-107">これらの記事には、一般的なメッセージ構造を示す例が用意されています。</span><span class="sxs-lookup"><span data-stu-id="2bb01-107">These articles provide examples that show common message structures.</span></span> <span data-ttu-id="2bb01-108">これらの例を使用して、ユニファイドメッセージング web サービス要求に対して実行できる操作について理解することができます。</span><span class="sxs-lookup"><span data-stu-id="2bb01-108">You can use these examples to learn about what you can do with a Unified Messaging web service request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="2bb01-109">Exchange 2010 以降のバージョンの Exchange では、次の理由から、ユニファイドメッセージング Web サービスの代わりに[Exchange Web サービス (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx)で使用できるユニファイドメッセージング操作を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="2bb01-109">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the Unified Messaging web service, for the following reasons:</span></span> 
> - <span data-ttu-id="2bb01-110">Ews ベースのユニファイドメッセージング機能には、EWS マネージ API でのファーストクラスのサポートが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2bb01-110">The EWS-based Unified Messaging features have first-class support in the EWS Managed API.</span></span> 
> - <span data-ttu-id="2bb01-111">Exchange 2010 以降のバージョンの Exchange では、新しいユニファイドメッセージング機能は EWS に追加されますが、ユニファイドメッセージング web サービスには追加されません。</span><span class="sxs-lookup"><span data-stu-id="2bb01-111">In versions of Exchange starting with Exchange 2010, new Unified Messaging features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="2bb01-112">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="2bb01-112">In this section</span></span>
<span data-ttu-id="2bb01-113"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="2bb01-113"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="2bb01-114">Disconnect 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="2bb01-114">Disconnect operation (UM web service)</span></span>](disconnect-operation-um-web-service.md)    
- [<span data-ttu-id="2bb01-115">GetCallInfo 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="2bb01-115">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)   
- [<span data-ttu-id="2bb01-116">GetUMProperties 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="2bb01-116">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)   
- [<span data-ttu-id="2bb01-117">IsUMEnabled 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="2bb01-117">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)   
- [<span data-ttu-id="2bb01-118">PlayOnPhone 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="2bb01-118">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)   
- [<span data-ttu-id="2bb01-119">Playon電話案内応答操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="2bb01-119">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)   
- [<span data-ttu-id="2bb01-120">ResetPIN 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="2bb01-120">ResetPIN operation (UM web service)</span></span>](resetpin-operation-um-web-service.md)   
- [<span data-ttu-id="2bb01-121">SetMissedCallNotificationEnabled 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="2bb01-121">SetMissedCallNotificationEnabled operation (UM web service)</span></span>](setmissedcallnotificationenabled-operation-um-web-service.md)  
- [<span data-ttu-id="2bb01-122">SetOofStatus 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="2bb01-122">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)    
- [<span data-ttu-id="2bb01-123">SetPlayOnPhoneDialString 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="2bb01-123">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)   
- [<span data-ttu-id="2bb01-124">SetTelephoneAccessFolderEmail 操作 (UM web サービス)</span><span class="sxs-lookup"><span data-stu-id="2bb01-124">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
    
## <a name="see-also"></a><span data-ttu-id="2bb01-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="2bb01-125">See also</span></span>

- [<span data-ttu-id="2bb01-126">Exchange 用ユニファイドメッセージング web サービスのリファレンス</span><span class="sxs-lookup"><span data-stu-id="2bb01-126">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
- [<span data-ttu-id="2bb01-127">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="2bb01-127">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="2bb01-128">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="2bb01-128">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

