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
description: RemoveDelegate 要素は、メールボックスから代理人を削除するための要求を定義します。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。
ms.openlocfilehash: eca357ad1ed2dc692f9f192b97abd3a5d765fafb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465521"
---
# <a name="removedelegate"></a><span data-ttu-id="00b1b-104">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="00b1b-104">RemoveDelegate</span></span>

<span data-ttu-id="00b1b-105">**Removedelegate**要素は、メールボックスから代理人を削除するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="00b1b-105">The **RemoveDelegate** element defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="00b1b-106">この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="00b1b-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<RemoveDelegate>
      <Mailbox/>
   <UserIds/>
</RemoveDelegate>
```

 <span data-ttu-id="00b1b-107">**RemoveDelegateType**</span><span class="sxs-lookup"><span data-stu-id="00b1b-107">**RemoveDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00b1b-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="00b1b-108">Attributes and elements</span></span>

<span data-ttu-id="00b1b-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="00b1b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00b1b-110">属性</span><span class="sxs-lookup"><span data-stu-id="00b1b-110">Attributes</span></span>

<span data-ttu-id="00b1b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="00b1b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00b1b-112">子要素</span><span class="sxs-lookup"><span data-stu-id="00b1b-112">Child elements</span></span>

|<span data-ttu-id="00b1b-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="00b1b-113">**Element**</span></span>|<span data-ttu-id="00b1b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="00b1b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00b1b-115">メールボックス</span><span class="sxs-lookup"><span data-stu-id="00b1b-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="00b1b-116">プリンシパルのメールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="00b1b-116">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="00b1b-117">UserIds</span><span class="sxs-lookup"><span data-stu-id="00b1b-117">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="00b1b-118">プリンシパルのメールボックスから削除するデリゲートユーザーの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="00b1b-118">Contains an array of delegate users to remove from a principal's mailbox.</span></span> <span data-ttu-id="00b1b-119">この要素は、Exchange 2007 SP1 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="00b1b-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00b1b-120">親要素</span><span class="sxs-lookup"><span data-stu-id="00b1b-120">Parent elements</span></span>

<span data-ttu-id="00b1b-121">なし。</span><span class="sxs-lookup"><span data-stu-id="00b1b-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="00b1b-122">注釈</span><span class="sxs-lookup"><span data-stu-id="00b1b-122">Remarks</span></span>

<span data-ttu-id="00b1b-123">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="00b1b-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00b1b-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="00b1b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00b1b-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="00b1b-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="00b1b-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="00b1b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="00b1b-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="00b1b-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="00b1b-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="00b1b-128">Validation File</span></span>  <br/> |<span data-ttu-id="00b1b-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="00b1b-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="00b1b-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="00b1b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="00b1b-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="00b1b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00b1b-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="00b1b-132">See also</span></span>



[<span data-ttu-id="00b1b-133">RemoveDelegate 操作</span><span class="sxs-lookup"><span data-stu-id="00b1b-133">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="00b1b-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="00b1b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

