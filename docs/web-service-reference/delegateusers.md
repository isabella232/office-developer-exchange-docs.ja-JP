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
description: DelegateUsers 要素には、メールボックス内の更新または追加する代理人の id が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: a078707ae6b1676ca5a32ba718add93debd498fe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759952"
---
# <a name="delegateusers"></a><span data-ttu-id="0ac70-104">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="0ac70-104">DelegateUsers</span></span>

<span data-ttu-id="0ac70-105">**DelegateUsers**要素には、メールボックス内の更新または追加する代理人の id が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0ac70-105">The **DelegateUsers** element contains the identities of delegates to add to or update in a mailbox.</span></span> <span data-ttu-id="0ac70-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0ac70-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUsers>
   <DelegateUser>
</DelegateUsers>
```

<span data-ttu-id="0ac70-107">**ArrayOfDelegateUserType**</span><span class="sxs-lookup"><span data-stu-id="0ac70-107">**ArrayOfDelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0ac70-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0ac70-108">Attributes and elements</span></span>

<span data-ttu-id="0ac70-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0ac70-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ac70-110">属性</span><span class="sxs-lookup"><span data-stu-id="0ac70-110">Attributes</span></span>

<span data-ttu-id="0ac70-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0ac70-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ac70-112">子要素</span><span class="sxs-lookup"><span data-stu-id="0ac70-112">Child elements</span></span>

|<span data-ttu-id="0ac70-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="0ac70-113">**Element**</span></span>|<span data-ttu-id="0ac70-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0ac70-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ac70-115">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="0ac70-115">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="0ac70-116">1 つのデリゲートに追加するか、メールボックスの更新を識別します。</span><span class="sxs-lookup"><span data-stu-id="0ac70-116">Identifies a single delegate to add to or update in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0ac70-117">親要素</span><span class="sxs-lookup"><span data-stu-id="0ac70-117">Parent elements</span></span>

|<span data-ttu-id="0ac70-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="0ac70-118">**Element**</span></span>|<span data-ttu-id="0ac70-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="0ac70-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ac70-120">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="0ac70-120">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="0ac70-121">メールボックスに代理人を追加する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="0ac70-121">Defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="0ac70-122">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0ac70-122">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="0ac70-123">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="0ac70-123">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="0ac70-124">メールボックスに代理人を更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="0ac70-124">Defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="0ac70-125">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0ac70-125">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0ac70-126">備考</span><span class="sxs-lookup"><span data-stu-id="0ac70-126">Remarks</span></span>

<span data-ttu-id="0ac70-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="0ac70-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ac70-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="0ac70-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ac70-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="0ac70-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0ac70-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0ac70-130">Schema Name</span></span>  <br/> |<span data-ttu-id="0ac70-131">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="0ac70-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0ac70-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0ac70-132">Validation File</span></span>  <br/> |<span data-ttu-id="0ac70-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0ac70-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0ac70-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0ac70-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="0ac70-135">False</span><span class="sxs-lookup"><span data-stu-id="0ac70-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ac70-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="0ac70-136">See also</span></span>

- [<span data-ttu-id="0ac70-137">AddDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="0ac70-137">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="0ac70-138">UpdateDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="0ac70-138">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="0ac70-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0ac70-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="0ac70-140">デリゲートを追加します。</span><span class="sxs-lookup"><span data-stu-id="0ac70-140">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

