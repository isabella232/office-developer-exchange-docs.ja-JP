---
title: IsSigned
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsSigned
api_type:
- schema
ms.assetid: a4f90fe5-2834-4621-9aa3-b561f74d4674
description: IsSigned 要素は、条件または例外を適用するために、受信メッセージが署名されている必要があるかどうかを示します。
ms.openlocfilehash: fe8551d01e6f9e813da8936f15b0b7ba1d4ce56c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455528"
---
# <a name="issigned"></a><span data-ttu-id="fc64e-103">IsSigned</span><span class="sxs-lookup"><span data-stu-id="fc64e-103">IsSigned</span></span>

<span data-ttu-id="fc64e-104">**Issigned**要素は、条件または例外を適用するために、受信メッセージが署名されている必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="fc64e-104">The **IsSigned** element indicates whether incoming messages must be signed in order for the condition or exception to apply.</span></span> 
  
```XML
<IsSigned>true | false</IsSigned>
```

 <span data-ttu-id="fc64e-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="fc64e-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc64e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fc64e-106">Attributes and elements</span></span>

<span data-ttu-id="fc64e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fc64e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc64e-108">属性</span><span class="sxs-lookup"><span data-stu-id="fc64e-108">Attributes</span></span>

<span data-ttu-id="fc64e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fc64e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc64e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fc64e-110">Child elements</span></span>

<span data-ttu-id="fc64e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fc64e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fc64e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="fc64e-112">Parent elements</span></span>

|<span data-ttu-id="fc64e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="fc64e-113">**Element**</span></span>|<span data-ttu-id="fc64e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="fc64e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc64e-115">条件</span><span class="sxs-lookup"><span data-stu-id="fc64e-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="fc64e-116">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="fc64e-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="fc64e-117">例外</span><span class="sxs-lookup"><span data-stu-id="fc64e-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="fc64e-118">受信トレイルールに対して使用可能なルールの例外条件をすべて表す例外を表します。</span><span class="sxs-lookup"><span data-stu-id="fc64e-118">Represents the exceptions that represent all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc64e-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fc64e-119">Text value</span></span>

<span data-ttu-id="fc64e-120">テキスト値が**true の場合**は、条件または例外を適用するために、メッセージを署名する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="fc64e-120">A text value of **true** indicates that the message must be signed in order for the condition or exception to apply.</span></span> <span data-ttu-id="fc64e-121">テキスト値が**false**の場合は、条件または例外を適用するためにメッセージを署名する必要がないことを示します。</span><span class="sxs-lookup"><span data-stu-id="fc64e-121">A text value of **false** indicates that the message does not have to be signed for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fc64e-122">注釈</span><span class="sxs-lookup"><span data-stu-id="fc64e-122">Remarks</span></span>

<span data-ttu-id="fc64e-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fc64e-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc64e-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fc64e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc64e-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="fc64e-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fc64e-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fc64e-126">Schema Name</span></span>  <br/> |<span data-ttu-id="fc64e-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="fc64e-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fc64e-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fc64e-128">Validation File</span></span>  <br/> |<span data-ttu-id="fc64e-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="fc64e-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fc64e-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fc64e-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc64e-131">正しい</span><span class="sxs-lookup"><span data-stu-id="fc64e-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc64e-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="fc64e-132">See also</span></span>



- [<span data-ttu-id="fc64e-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="fc64e-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

