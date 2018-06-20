---
title: ReceiveCopiesOfMeetingMessages
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReceiveCopiesOfMeetingMessages
api_type:
- schema
ms.assetid: 65217ca8-6aea-47eb-a989-e6cce25f5f09
description: ReceiveCopiesOfMeetingMessages 要素は、代理人が会議に関連するプリンシパルにアドレス指定されたメッセージのコピーを受け取るかどうかを示します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: e39a5d3255268b418fa956959da5ae0ea062d831
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832967"
---
# <a name="receivecopiesofmeetingmessages"></a><span data-ttu-id="db100-104">ReceiveCopiesOfMeetingMessages</span><span class="sxs-lookup"><span data-stu-id="db100-104">ReceiveCopiesOfMeetingMessages</span></span>

<span data-ttu-id="db100-105">**ReceiveCopiesOfMeetingMessages**要素は、代理人が会議に関連するプリンシパルにアドレス指定されたメッセージのコピーを受け取るかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="db100-105">The **ReceiveCopiesOfMeetingMessages** element indicates whether a delegate receives copies of meeting-related messages that are addressed to the principal.</span></span> <span data-ttu-id="db100-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="db100-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<ReceiveCopiesOfMeetingMessages>true or false</ReceiveCopiesOfMeetingMessages>
```

 <span data-ttu-id="db100-107">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="db100-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db100-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="db100-108">Attributes and elements</span></span>

<span data-ttu-id="db100-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="db100-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db100-110">属性</span><span class="sxs-lookup"><span data-stu-id="db100-110">Attributes</span></span>

<span data-ttu-id="db100-111">なし。</span><span class="sxs-lookup"><span data-stu-id="db100-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db100-112">子要素</span><span class="sxs-lookup"><span data-stu-id="db100-112">Child elements</span></span>

<span data-ttu-id="db100-113">なし。</span><span class="sxs-lookup"><span data-stu-id="db100-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="db100-114">親要素</span><span class="sxs-lookup"><span data-stu-id="db100-114">Parent elements</span></span>

|<span data-ttu-id="db100-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="db100-115">**Element**</span></span>|<span data-ttu-id="db100-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="db100-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db100-117">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="db100-117">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="db100-118">1 つのデリゲートを追加するメールボックスの更新を識別します。</span><span class="sxs-lookup"><span data-stu-id="db100-118">Identifies a single delegate to add or update in a mailbox.</span></span> <span data-ttu-id="db100-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="db100-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="db100-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="db100-120">Text value</span></span>

<span data-ttu-id="db100-121">**True**の場合、テキスト値では、代理人が会議のメッセージのコピーを受信することを示します。</span><span class="sxs-lookup"><span data-stu-id="db100-121">A text value of **true** indicates that a delegate receives a copy of meeting messages.</span></span> <span data-ttu-id="db100-122">**False**のテキスト値では、代理人が会議のメッセージのコピーを受信していないことを示します。</span><span class="sxs-lookup"><span data-stu-id="db100-122">A text value of **false** indicates that a delegate does not receive a copy of meeting messages.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="db100-123">備考</span><span class="sxs-lookup"><span data-stu-id="db100-123">Remarks</span></span>

<span data-ttu-id="db100-124">**ReceiveCopiesOfMeetingMessages**を**false**に設定すると、デリゲートは、プリンシパルの代わりにメッセージを送信できますが、会議に関連するメッセージは表示されませんが。</span><span class="sxs-lookup"><span data-stu-id="db100-124">When **ReceiveCopiesOfMeetingMessages** is set to **false**, the delegate can still send message on behalf of the principal, but will not receive any meeting-related messages.</span></span>
  
<span data-ttu-id="db100-125">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="db100-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db100-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="db100-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db100-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="db100-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="db100-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="db100-128">Schema Name</span></span>  <br/> |<span data-ttu-id="db100-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="db100-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="db100-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="db100-130">Validation File</span></span>  <br/> |<span data-ttu-id="db100-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="db100-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="db100-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="db100-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="db100-133">False</span><span class="sxs-lookup"><span data-stu-id="db100-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db100-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="db100-134">See also</span></span>



[<span data-ttu-id="db100-135">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="db100-135">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="db100-136">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="db100-136">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="db100-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="db100-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="db100-138">デリゲートを追加します。</span><span class="sxs-lookup"><span data-stu-id="db100-138">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

