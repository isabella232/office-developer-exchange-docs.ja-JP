---
title: ユニファイド メッセージング web サービスの操作の交換
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
description: Exchange ユニファイド メッセージングの web サービスの操作に関する参照情報を検索します。
ms.openlocfilehash: bd86a4ab2de58e5f04a8d37f17196040bcf38b97
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354359"
---
# <a name="unified-messaging-web-service-operations-for-exchange"></a><span data-ttu-id="d1074-103">ユニファイド メッセージング web サービスの操作の交換</span><span class="sxs-lookup"><span data-stu-id="d1074-103">Unified Messaging web service operations for Exchange</span></span>

<span data-ttu-id="d1074-104">Exchange ユニファイド メッセージングの web サービスの操作に関する参照情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="d1074-104">Find reference information for the Unified Messaging web service operations in Exchange.</span></span>
  
<span data-ttu-id="d1074-105">ユニファイド メッセージング web サービスは、ユニファイド メッセージングのプロパティを変更する、ボイス メール メッセージの再生、記録、あいさつ文、およびテレフォニー デバイス経由でメールボックスのアイテムを指定のクライアント アプリケーションを有効にするさまざまな処理を提供します。</span><span class="sxs-lookup"><span data-stu-id="d1074-105">The Unified Messaging web service provides many operations that enable client applications to read and change Unified Messaging properties, play voice mail messages, record greetings, and dictate mailbox items over telephony devices.</span></span> <span data-ttu-id="d1074-106">このセクションの記事では、操作の要求と応答メッセージの全体的な構造についての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="d1074-106">The articles in this section provide information about the overall structure of the request and response messages for the operations.</span></span> <span data-ttu-id="d1074-107">これらの資料では、一般的なメッセージの構造を表示する例を示します。</span><span class="sxs-lookup"><span data-stu-id="d1074-107">These articles provide examples that show common message structures.</span></span> <span data-ttu-id="d1074-108">これらの例を使用すると、ユニファイド メッセージングの web サービス要求を行うことができますについて説明します。</span><span class="sxs-lookup"><span data-stu-id="d1074-108">You can use these examples to learn about what you can do with a Unified Messaging web service request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="d1074-109">Exchange が Exchange 2010 以降のバージョンでは、ユニファイド メッセージング web サービスで、次の理由からではなく[Exchange Web サービス (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx)で利用可能なユニファイド メッセージングの操作を使用することお勧めします。</span><span class="sxs-lookup"><span data-stu-id="d1074-109">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the Unified Messaging web service, for the following reasons:</span></span> 
> - <span data-ttu-id="d1074-110">EWS ベースのユニファイド メッセージング機能では、EWS のマネージ API でファースト クラスのサポートがあります。</span><span class="sxs-lookup"><span data-stu-id="d1074-110">The EWS-based Unified Messaging features have first-class support in the EWS Managed API.</span></span> 
> - <span data-ttu-id="d1074-111">Exchange が Exchange 2010 以降のバージョンでは、ユニファイド メッセージング web サービスではなく、EWS にユニファイド メッセージングの新機能が追加されます。</span><span class="sxs-lookup"><span data-stu-id="d1074-111">In versions of Exchange starting with Exchange 2010, new Unified Messaging features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="d1074-112">このセクションの内容</span><span class="sxs-lookup"><span data-stu-id="d1074-112">In this section</span></span>
<span data-ttu-id="d1074-113"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="d1074-113"></span></span>

- [<span data-ttu-id="d1074-114">切断操作 (UM Web サービス)</span><span class="sxs-lookup"><span data-stu-id="d1074-114">Disconnect operation (UM web service)</span></span>](disconnect-operation-um-web-service.md)    
- [<span data-ttu-id="d1074-115">GetCallInfo 操作 (UM Web サービス)</span><span class="sxs-lookup"><span data-stu-id="d1074-115">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)   
- [<span data-ttu-id="d1074-116">GetUMProperties 操作 (UM Web サービス)</span><span class="sxs-lookup"><span data-stu-id="d1074-116">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)   
- [<span data-ttu-id="d1074-117">IsUMEnabled 操作 (UM Web サービス)</span><span class="sxs-lookup"><span data-stu-id="d1074-117">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)   
- [<span data-ttu-id="d1074-118">PlayOnPhone 操作 (UM Web サービス)</span><span class="sxs-lookup"><span data-stu-id="d1074-118">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)   
- [<span data-ttu-id="d1074-119">PlayOnPhoneGreeting 操作 (UM Web サービス)</span><span class="sxs-lookup"><span data-stu-id="d1074-119">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)   
- [<span data-ttu-id="d1074-120">ResetPIN 操作 (UM Web サービス)</span><span class="sxs-lookup"><span data-stu-id="d1074-120">ResetPIN operation (UM web service)</span></span>](resetpin-operation-um-web-service.md)   
- [<span data-ttu-id="d1074-121">SetMissedCallNotificationEnabled 操作 (UM Web サービス)</span><span class="sxs-lookup"><span data-stu-id="d1074-121">SetMissedCallNotificationEnabled operation (UM web service)</span></span>](setmissedcallnotificationenabled-operation-um-web-service.md)  
- [<span data-ttu-id="d1074-122">SetOofStatus 操作 (UM Web サービス)</span><span class="sxs-lookup"><span data-stu-id="d1074-122">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)    
- [<span data-ttu-id="d1074-123">SetPlayOnPhoneDialString 操作 (UM Web サービス)</span><span class="sxs-lookup"><span data-stu-id="d1074-123">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)   
- [<span data-ttu-id="d1074-124">SetTelephoneAccessFolderEmail 操作 (UM Web サービス)</span><span class="sxs-lookup"><span data-stu-id="d1074-124">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
    
## <a name="see-also"></a><span data-ttu-id="d1074-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="d1074-125">See also</span></span>

- [<span data-ttu-id="d1074-126">Exchange ユニファイド メッセージング web サービス リファレンス</span><span class="sxs-lookup"><span data-stu-id="d1074-126">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
- [<span data-ttu-id="d1074-127">Exchange の自動検出</span><span class="sxs-lookup"><span data-stu-id="d1074-127">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="d1074-128">Exchange で Web サービスの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="d1074-128">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

