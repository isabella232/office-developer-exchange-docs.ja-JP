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
description: SendNotification 要素には、Microsoft Exchange Server 2007 を実行しているコンピューターによってクライアントアプリケーションに送信されるプッシュ通知が含まれています。
ms.openlocfilehash: 49f2f6cb7f5c8e1171b54ff965ee1d22accc9bf2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462116"
---
# <a name="sendnotification"></a><span data-ttu-id="83b70-103">SendNotification</span><span class="sxs-lookup"><span data-stu-id="83b70-103">SendNotification</span></span>

<span data-ttu-id="83b70-104">**Sendnotification**要素には、Microsoft Exchange Server 2007 を実行しているコンピューターによってクライアントアプリケーションに送信されるプッシュ通知が含まれています。</span><span class="sxs-lookup"><span data-stu-id="83b70-104">The **SendNotification** element contains the push notifications that are sent by the computer that is running Microsoft Exchange Server 2007 to the client application.</span></span> 
  
```xml
<SendNotification>
   <ResponseMessages/>
</SendNotification>
```

 <span data-ttu-id="83b70-105">**SendNotificationResponseType**</span><span class="sxs-lookup"><span data-stu-id="83b70-105">**SendNotificationResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83b70-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="83b70-106">Attributes and elements</span></span>

<span data-ttu-id="83b70-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="83b70-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83b70-108">属性</span><span class="sxs-lookup"><span data-stu-id="83b70-108">Attributes</span></span>

<span data-ttu-id="83b70-109">なし。</span><span class="sxs-lookup"><span data-stu-id="83b70-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83b70-110">子要素</span><span class="sxs-lookup"><span data-stu-id="83b70-110">Child elements</span></span>

|<span data-ttu-id="83b70-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="83b70-111">**Element**</span></span>|<span data-ttu-id="83b70-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="83b70-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83b70-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="83b70-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="83b70-114">クライアントアクセスサーバーによって送信されるプッシュ通知が含まれます。</span><span class="sxs-lookup"><span data-stu-id="83b70-114">Contains the push notifications that are sent by the Client Access server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="83b70-115">親要素</span><span class="sxs-lookup"><span data-stu-id="83b70-115">Parent elements</span></span>

<span data-ttu-id="83b70-116">なし。</span><span class="sxs-lookup"><span data-stu-id="83b70-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="83b70-117">注釈</span><span class="sxs-lookup"><span data-stu-id="83b70-117">Remarks</span></span>

<span data-ttu-id="83b70-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="83b70-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83b70-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="83b70-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83b70-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="83b70-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="83b70-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="83b70-121">Schema Name</span></span>  <br/> |<span data-ttu-id="83b70-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="83b70-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="83b70-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="83b70-123">Validation File</span></span>  <br/> |<span data-ttu-id="83b70-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="83b70-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="83b70-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="83b70-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="83b70-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="83b70-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="83b70-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="83b70-127">See also</span></span>



- [<span data-ttu-id="83b70-128">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="83b70-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="83b70-129">EWS でのイベント通知</span><span class="sxs-lookup"><span data-stu-id="83b70-129">Event notifications in EWS</span></span>](https://msdn.microsoft.com/library/4fd4b351-d35c-4ccc-9ed9-878932ab9d50%28Office.15%29.aspx)
  
[<span data-ttu-id="83b70-130">プッシュ通知のサンプル アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83b70-130">Push Notification Sample Application</span></span>](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

