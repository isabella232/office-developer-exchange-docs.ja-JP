---
title: RemoveOutlookRuleBlob
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveOutlookRuleBlob
api_type:
- schema
ms.assetid: 69614475-8bd3-4475-b988-614fe9cad8ef
description: RemoveOutlookRuleBlob 要素は、Microsoft Outlook のルール blob を削除するかどうかを示します。
ms.openlocfilehash: b4202ab52bf16d1ad1546ec963cd8b9dacd2bd63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467670"
---
# <a name="removeoutlookruleblob"></a><span data-ttu-id="d53c9-103">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="d53c9-103">RemoveOutlookRuleBlob</span></span>

<span data-ttu-id="d53c9-104">**Removeoutlookruleblob**要素は、Microsoft Outlook のルール blob を削除するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d53c9-104">The **RemoveOutlookRuleBlob** element indicates whether to remove the Microsoft Outlook rule blob.</span></span> 
  
[<span data-ttu-id="d53c9-105">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="d53c9-105">UpdateInboxRules</span></span>](updateinboxrules.md)
  
[<span data-ttu-id="d53c9-106">RemoveOutlookRuleBlob</span><span class="sxs-lookup"><span data-stu-id="d53c9-106">RemoveOutlookRuleBlob</span></span>](removeoutlookruleblob.md)
  
```XML
<RemoveOutlookRuleBlob>true | false</RemoveOutlookRuleBlob>
```

 <span data-ttu-id="d53c9-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d53c9-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d53c9-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d53c9-108">Attributes and elements</span></span>

<span data-ttu-id="d53c9-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d53c9-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d53c9-110">属性</span><span class="sxs-lookup"><span data-stu-id="d53c9-110">Attributes</span></span>

<span data-ttu-id="d53c9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d53c9-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d53c9-112">子要素</span><span class="sxs-lookup"><span data-stu-id="d53c9-112">Child elements</span></span>

<span data-ttu-id="d53c9-113">なし。</span><span class="sxs-lookup"><span data-stu-id="d53c9-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d53c9-114">親要素</span><span class="sxs-lookup"><span data-stu-id="d53c9-114">Parent elements</span></span>

|<span data-ttu-id="d53c9-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="d53c9-115">**Element**</span></span>|<span data-ttu-id="d53c9-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="d53c9-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d53c9-117">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="d53c9-117">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="d53c9-118">サーバーストア内のメールボックスの受信トレイルールを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="d53c9-118">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d53c9-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d53c9-119">Text value</span></span>

<span data-ttu-id="d53c9-120">テキスト値が**true の場合**は、Outlook ルール blob を削除する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="d53c9-120">A text value of **true** indicates that the Outlook rule blob should be removed.</span></span> <span data-ttu-id="d53c9-121">テキスト値が**false**の場合は、Outlook ルール blob を削除しないようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d53c9-121">A text value of **false** indicates that the Outlook rule blob should not be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d53c9-122">注釈</span><span class="sxs-lookup"><span data-stu-id="d53c9-122">Remarks</span></span>

<span data-ttu-id="d53c9-123">受信トレイルールの更新を許可するには、この要素を**true**に設定します。</span><span class="sxs-lookup"><span data-stu-id="d53c9-123">Set this element to **true** to allow for an Inbox rule update.</span></span> 
  
<span data-ttu-id="d53c9-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d53c9-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d53c9-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d53c9-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d53c9-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="d53c9-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d53c9-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d53c9-127">Schema Name</span></span>  <br/> |<span data-ttu-id="d53c9-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d53c9-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="d53c9-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d53c9-129">Validation File</span></span>  <br/> |<span data-ttu-id="d53c9-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d53c9-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d53c9-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d53c9-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="d53c9-132">正しい</span><span class="sxs-lookup"><span data-stu-id="d53c9-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d53c9-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="d53c9-133">See also</span></span>



[<span data-ttu-id="d53c9-134">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="d53c9-134">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)


- [<span data-ttu-id="d53c9-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d53c9-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

