---
title: ユーザー Id
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
description: 要素の配列を格納するユーザー Id を取得またはプリンシパルのメールボックスから削除するユーザーを委任します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 277ae96fdbc30f1b39ef20553e10ff1de3ff7a8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839936"
---
# <a name="userids"></a><span data-ttu-id="11230-104">ユーザー Id</span><span class="sxs-lookup"><span data-stu-id="11230-104">UserIds</span></span>

<span data-ttu-id="11230-105">**ユーザー Id**要素には、取得、またはプリンシパルのメールボックスから削除する代理人のユーザーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="11230-105">The **UserIds** element contains an array of delegate users to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="11230-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="11230-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<UserIds>
   <UserId/>
</UserIds>
```

 <span data-ttu-id="11230-107">**ArrayOfUserIdType**</span><span class="sxs-lookup"><span data-stu-id="11230-107">**ArrayOfUserIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11230-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="11230-108">Attributes and elements</span></span>

<span data-ttu-id="11230-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="11230-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11230-110">属性</span><span class="sxs-lookup"><span data-stu-id="11230-110">Attributes</span></span>

<span data-ttu-id="11230-111">なし。</span><span class="sxs-lookup"><span data-stu-id="11230-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11230-112">子要素</span><span class="sxs-lookup"><span data-stu-id="11230-112">Child elements</span></span>

|<span data-ttu-id="11230-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="11230-113">**Element**</span></span>|<span data-ttu-id="11230-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="11230-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11230-115">ユーザー Id</span><span class="sxs-lookup"><span data-stu-id="11230-115">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="11230-116">取得またはプリンシパルのメールボックスから削除するデリゲートを指定します。</span><span class="sxs-lookup"><span data-stu-id="11230-116">Identifies a delegate to get or remove from a principal's mailbox.</span></span> <span data-ttu-id="11230-117">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="11230-117">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="11230-118">親要素</span><span class="sxs-lookup"><span data-stu-id="11230-118">Parent elements</span></span>

|<span data-ttu-id="11230-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="11230-119">**Element**</span></span>|<span data-ttu-id="11230-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="11230-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11230-121">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="11230-121">GetDelegate</span></span>](getdelegate.md) <br/> |<span data-ttu-id="11230-122">メールボックスに代理人についての情報を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="11230-122">Defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="11230-123">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="11230-123">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="11230-124">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="11230-124">RemoveDelegate</span></span>](removedelegate.md) <br/> |<span data-ttu-id="11230-125">メールボックスからデリゲートを削除する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="11230-125">Defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="11230-126">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="11230-126">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="11230-127">備考</span><span class="sxs-lookup"><span data-stu-id="11230-127">Remarks</span></span>

<span data-ttu-id="11230-128">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="11230-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11230-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="11230-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11230-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="11230-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="11230-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="11230-131">Schema Name</span></span>  <br/> |<span data-ttu-id="11230-132">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="11230-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="11230-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="11230-133">Validation File</span></span>  <br/> |<span data-ttu-id="11230-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="11230-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="11230-135">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="11230-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="11230-136">False</span><span class="sxs-lookup"><span data-stu-id="11230-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11230-137">関連項目</span><span class="sxs-lookup"><span data-stu-id="11230-137">See also</span></span>



[<span data-ttu-id="11230-138">GetDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="11230-138">GetDelegate operation</span></span>](getdelegate-operation.md)
  
[<span data-ttu-id="11230-139">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="11230-139">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="11230-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="11230-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

