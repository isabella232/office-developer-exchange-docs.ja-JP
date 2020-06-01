---
title: DelegateUsers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUsers
api_type:
- schema
ms.assetid: f30f80d9-20c8-41cc-afc7-a5eec1e0c5ea
description: DelegateUsers 要素には、メールボックスに追加または更新する代理人の id が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 69f5aab65634f41ec0f820da05dee79a300fb32e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457376"
---
# <a name="delegateusers"></a><span data-ttu-id="6c07a-104">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="6c07a-104">DelegateUsers</span></span>

<span data-ttu-id="6c07a-105">**DelegateUsers**要素には、メールボックスに追加または更新する代理人の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6c07a-105">The **DelegateUsers** element contains the identities of delegates to add to or update in a mailbox.</span></span> <span data-ttu-id="6c07a-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6c07a-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUsers>
   <DelegateUser>
</DelegateUsers>
```

<span data-ttu-id="6c07a-107">**ArrayOfDelegateUserType**</span><span class="sxs-lookup"><span data-stu-id="6c07a-107">**ArrayOfDelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6c07a-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6c07a-108">Attributes and elements</span></span>

<span data-ttu-id="6c07a-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c07a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c07a-110">属性</span><span class="sxs-lookup"><span data-stu-id="6c07a-110">Attributes</span></span>

<span data-ttu-id="6c07a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6c07a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c07a-112">子要素</span><span class="sxs-lookup"><span data-stu-id="6c07a-112">Child elements</span></span>

|<span data-ttu-id="6c07a-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="6c07a-113">**Element**</span></span>|<span data-ttu-id="6c07a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c07a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c07a-115">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="6c07a-115">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="6c07a-116">メールボックスに追加または更新する単一の代理人を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c07a-116">Identifies a single delegate to add to or update in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6c07a-117">親要素</span><span class="sxs-lookup"><span data-stu-id="6c07a-117">Parent elements</span></span>

|<span data-ttu-id="6c07a-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="6c07a-118">**Element**</span></span>|<span data-ttu-id="6c07a-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="6c07a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c07a-120">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="6c07a-120">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="6c07a-121">メールボックスに代理人を追加するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6c07a-121">Defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="6c07a-122">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6c07a-122">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="6c07a-123">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="6c07a-123">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="6c07a-124">メールボックスの代理人を更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6c07a-124">Defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="6c07a-125">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6c07a-125">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6c07a-126">注釈</span><span class="sxs-lookup"><span data-stu-id="6c07a-126">Remarks</span></span>

<span data-ttu-id="6c07a-127">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="6c07a-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c07a-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6c07a-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c07a-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="6c07a-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6c07a-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6c07a-130">Schema Name</span></span>  <br/> |<span data-ttu-id="6c07a-131">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="6c07a-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6c07a-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6c07a-132">Validation File</span></span>  <br/> |<span data-ttu-id="6c07a-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6c07a-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6c07a-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6c07a-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="6c07a-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="6c07a-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c07a-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c07a-136">See also</span></span>

- [<span data-ttu-id="6c07a-137">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="6c07a-137">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="6c07a-138">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="6c07a-138">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="6c07a-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6c07a-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="6c07a-140">代理人の追加</span><span class="sxs-lookup"><span data-stu-id="6c07a-140">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

