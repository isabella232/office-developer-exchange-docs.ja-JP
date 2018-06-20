---
title: SendNotification
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendNotification
api_type:
- schema
ms.assetid: e45c4451-a286-4aec-a691-119ec41c58e0
description: SendNotification 要素には、クライアント アプリケーションを Microsoft Exchange Server 2007 を実行しているコンピューターから送信されるプッシュ通知が含まれています。
ms.openlocfilehash: 2288dbb5cf97b57a64b3c645eb72836342f4c178
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833345"
---
# <a name="sendnotification"></a><span data-ttu-id="7bda7-103">SendNotification</span><span class="sxs-lookup"><span data-stu-id="7bda7-103">SendNotification</span></span>

<span data-ttu-id="7bda7-104">**SendNotification**要素には、クライアント アプリケーションを Microsoft Exchange Server 2007 を実行しているコンピューターから送信されるプッシュ通知が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7bda7-104">The **SendNotification** element contains the push notifications that are sent by the computer that is running Microsoft Exchange Server 2007 to the client application.</span></span> 
  
```xml
<SendNotification>
   <ResponseMessages/>
</SendNotification>
```

 <span data-ttu-id="7bda7-105">**SendNotificationResponseType**</span><span class="sxs-lookup"><span data-stu-id="7bda7-105">**SendNotificationResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7bda7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7bda7-106">Attributes and elements</span></span>

<span data-ttu-id="7bda7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7bda7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7bda7-108">属性</span><span class="sxs-lookup"><span data-stu-id="7bda7-108">Attributes</span></span>

<span data-ttu-id="7bda7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7bda7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7bda7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7bda7-110">Child elements</span></span>

|<span data-ttu-id="7bda7-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="7bda7-111">**Element**</span></span>|<span data-ttu-id="7bda7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7bda7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7bda7-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7bda7-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7bda7-114">クライアント アクセス サーバーによって送信されるプッシュ通知が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7bda7-114">Contains the push notifications that are sent by the Client Access server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7bda7-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7bda7-115">Parent elements</span></span>

<span data-ttu-id="7bda7-116">なし。</span><span class="sxs-lookup"><span data-stu-id="7bda7-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7bda7-117">備考</span><span class="sxs-lookup"><span data-stu-id="7bda7-117">Remarks</span></span>

<span data-ttu-id="7bda7-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="7bda7-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7bda7-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="7bda7-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7bda7-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="7bda7-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7bda7-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7bda7-121">Schema Name</span></span>  <br/> |<span data-ttu-id="7bda7-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7bda7-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7bda7-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7bda7-123">Validation File</span></span>  <br/> |<span data-ttu-id="7bda7-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7bda7-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7bda7-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7bda7-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="7bda7-126">False</span><span class="sxs-lookup"><span data-stu-id="7bda7-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7bda7-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="7bda7-127">See also</span></span>



- [<span data-ttu-id="7bda7-128">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7bda7-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="7bda7-129">EWS でのイベントの通知</span><span class="sxs-lookup"><span data-stu-id="7bda7-129">Event notifications in EWS</span></span>](http://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)
  
[<span data-ttu-id="7bda7-130">プッシュ通知のサンプル アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7bda7-130">Push Notification Sample Application</span></span>](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

