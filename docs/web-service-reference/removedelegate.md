---
title: RemoveDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegate
api_type:
- schema
ms.assetid: f21c5171-62e7-47c8-99b1-22e1ff5883bb
description: RemoveDelegate 要素は、メールボックスからデリゲートを削除する要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: 27618b1767c99b26a5f4c06e97a20e063b598d9d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833085"
---
# <a name="removedelegate"></a><span data-ttu-id="f3ee4-104">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="f3ee4-104">RemoveDelegate</span></span>

<span data-ttu-id="f3ee4-105">**RemoveDelegate**要素は、メールボックスからデリゲートを削除する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f3ee4-105">The **RemoveDelegate** element defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="f3ee4-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f3ee4-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<RemoveDelegate>
      <Mailbox/>
   <UserIds/>
</RemoveDelegate>
```

 <span data-ttu-id="f3ee4-107">**RemoveDelegateType**</span><span class="sxs-lookup"><span data-stu-id="f3ee4-107">**RemoveDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3ee4-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f3ee4-108">Attributes and elements</span></span>

<span data-ttu-id="f3ee4-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f3ee4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3ee4-110">属性</span><span class="sxs-lookup"><span data-stu-id="f3ee4-110">Attributes</span></span>

<span data-ttu-id="f3ee4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f3ee4-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3ee4-112">子要素</span><span class="sxs-lookup"><span data-stu-id="f3ee4-112">Child elements</span></span>

|<span data-ttu-id="f3ee4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f3ee4-113">**Element**</span></span>|<span data-ttu-id="f3ee4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f3ee4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3ee4-115">メールボックス</span><span class="sxs-lookup"><span data-stu-id="f3ee4-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="f3ee4-116">主体のメールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="f3ee4-116">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f3ee4-117">ユーザー Id</span><span class="sxs-lookup"><span data-stu-id="f3ee4-117">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="f3ee4-118">主体のメールボックスから削除する代理人のユーザーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3ee4-118">Contains an array of delegate users to remove from a principal's mailbox.</span></span> <span data-ttu-id="f3ee4-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f3ee4-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f3ee4-120">親要素</span><span class="sxs-lookup"><span data-stu-id="f3ee4-120">Parent elements</span></span>

<span data-ttu-id="f3ee4-121">なし。</span><span class="sxs-lookup"><span data-stu-id="f3ee4-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f3ee4-122">備考</span><span class="sxs-lookup"><span data-stu-id="f3ee4-122">Remarks</span></span>

<span data-ttu-id="f3ee4-123">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f3ee4-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3ee4-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="f3ee4-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3ee4-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="f3ee4-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f3ee4-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f3ee4-126">Schema Name</span></span>  <br/> |<span data-ttu-id="f3ee4-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f3ee4-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f3ee4-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f3ee4-128">Validation File</span></span>  <br/> |<span data-ttu-id="f3ee4-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f3ee4-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f3ee4-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f3ee4-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3ee4-131">False</span><span class="sxs-lookup"><span data-stu-id="f3ee4-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3ee4-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="f3ee4-132">See also</span></span>



[<span data-ttu-id="f3ee4-133">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="f3ee4-133">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="f3ee4-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f3ee4-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

