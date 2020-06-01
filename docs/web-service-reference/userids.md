---
title: UserIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserIds
api_type:
- schema
ms.assetid: 78a09c3a-1646-4c55-95a2-1109fb11e1c6
description: UserIds 要素には、プリンシパルのメールボックスから取得または削除するデリゲートユーザーの配列が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: de4661226c154ef0d2d5ac55c57405e20c4d2aee
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459778"
---
# <a name="userids"></a><span data-ttu-id="2bb23-104">UserIds</span><span class="sxs-lookup"><span data-stu-id="2bb23-104">UserIds</span></span>

<span data-ttu-id="2bb23-105">**UserIds**要素には、プリンシパルのメールボックスから取得または削除するデリゲートユーザーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2bb23-105">The **UserIds** element contains an array of delegate users to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="2bb23-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2bb23-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UserIds>
   <UserId/>
</UserIds>
```

 <span data-ttu-id="2bb23-107">**ArrayOfUserIdType**</span><span class="sxs-lookup"><span data-stu-id="2bb23-107">**ArrayOfUserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2bb23-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2bb23-108">Attributes and elements</span></span>

<span data-ttu-id="2bb23-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2bb23-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2bb23-110">属性</span><span class="sxs-lookup"><span data-stu-id="2bb23-110">Attributes</span></span>

<span data-ttu-id="2bb23-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2bb23-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2bb23-112">子要素</span><span class="sxs-lookup"><span data-stu-id="2bb23-112">Child elements</span></span>

|<span data-ttu-id="2bb23-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="2bb23-113">**Element**</span></span>|<span data-ttu-id="2bb23-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="2bb23-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2bb23-115">UserId</span><span class="sxs-lookup"><span data-stu-id="2bb23-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="2bb23-116">プリンシパルのメールボックスから取得または削除する代理人を指定します。</span><span class="sxs-lookup"><span data-stu-id="2bb23-116">Identifies a delegate to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="2bb23-117">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2bb23-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2bb23-118">親要素</span><span class="sxs-lookup"><span data-stu-id="2bb23-118">Parent elements</span></span>

|<span data-ttu-id="2bb23-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="2bb23-119">**Element**</span></span>|<span data-ttu-id="2bb23-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="2bb23-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2bb23-121">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="2bb23-121">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="2bb23-122">メールボックスへの代理人に関する情報を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="2bb23-122">Defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="2bb23-123">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2bb23-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="2bb23-124">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="2bb23-124">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="2bb23-125">メールボックスから代理人を削除するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="2bb23-125">Defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="2bb23-126">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2bb23-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2bb23-127">注釈</span><span class="sxs-lookup"><span data-stu-id="2bb23-127">Remarks</span></span>

<span data-ttu-id="2bb23-128">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="2bb23-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2bb23-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2bb23-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2bb23-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="2bb23-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2bb23-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2bb23-131">Schema Name</span></span>  <br/> |<span data-ttu-id="2bb23-132">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2bb23-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2bb23-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2bb23-133">Validation File</span></span>  <br/> |<span data-ttu-id="2bb23-134">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2bb23-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2bb23-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2bb23-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="2bb23-136">正しくない</span><span class="sxs-lookup"><span data-stu-id="2bb23-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2bb23-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="2bb23-137">See also</span></span>



[<span data-ttu-id="2bb23-138">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="2bb23-138">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="2bb23-139">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="2bb23-139">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="2bb23-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2bb23-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

