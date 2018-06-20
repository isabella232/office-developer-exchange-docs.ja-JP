---
title: ExchangeStoreId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5acceb42-a757-4c74-ab1c-b1abf7bf1e0a
description: ExchangeStoreId 要素は、インスタント メッセージング (IM) グループの識別子を指定します。
ms.openlocfilehash: 815e9c2f368558ea38efce3671dbdc33d4d97168
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760361"
---
# <a name="exchangestoreid"></a><span data-ttu-id="7b819-103">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="7b819-103">ExchangeStoreId</span></span>

<span data-ttu-id="7b819-104">**ExchangeStoreId**要素は、インスタント メッセージング (IM) グループの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="7b819-104">The **ExchangeStoreId** element specifies the instant messaging (IM) group identifier.</span></span> 
  
```XML
<ExchangeStoreId Id="" ChangeKey=""/>
```

 <span data-ttu-id="7b819-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="7b819-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b819-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7b819-106">Attributes and elements</span></span>

<span data-ttu-id="7b819-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7b819-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b819-108">属性</span><span class="sxs-lookup"><span data-stu-id="7b819-108">Attributes</span></span>

|<span data-ttu-id="7b819-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="7b819-109">**Attribute**</span></span>|<span data-ttu-id="7b819-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="7b819-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7b819-111">ID</span><span class="sxs-lookup"><span data-stu-id="7b819-111">Id</span></span>  <br/> |<span data-ttu-id="7b819-112">**Id**属性のテキスト値は、グループの識別子です。</span><span class="sxs-lookup"><span data-stu-id="7b819-112">The text value of the **Id** attribute is the identifier of the group.</span></span>  <br/> |
|<span data-ttu-id="7b819-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="7b819-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="7b819-114">**変更キー**属性のテキスト値は、グループのキーの変更です。</span><span class="sxs-lookup"><span data-stu-id="7b819-114">The text value of the **ChangeKey** attribute is the change key of the group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7b819-115">子要素</span><span class="sxs-lookup"><span data-stu-id="7b819-115">Child elements</span></span>

<span data-ttu-id="7b819-116">なし。</span><span class="sxs-lookup"><span data-stu-id="7b819-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7b819-117">親要素</span><span class="sxs-lookup"><span data-stu-id="7b819-117">Parent elements</span></span>

|<span data-ttu-id="7b819-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="7b819-118">**Element**</span></span>|<span data-ttu-id="7b819-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="7b819-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b819-120">ImGroup</span><span class="sxs-lookup"><span data-stu-id="7b819-120">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="7b819-121">インスタント メッセージングのグループを表します。</span><span class="sxs-lookup"><span data-stu-id="7b819-121">Represents an instant messaging group.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7b819-122">備考</span><span class="sxs-lookup"><span data-stu-id="7b819-122">Remarks</span></span>

<span data-ttu-id="7b819-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7b819-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7b819-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7b819-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b819-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="7b819-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b819-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="7b819-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7b819-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7b819-127">Schema Name</span></span>  <br/> |<span data-ttu-id="7b819-128">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="7b819-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="7b819-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7b819-129">Validation File</span></span>  <br/> |<span data-ttu-id="7b819-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="7b819-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="7b819-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7b819-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7b819-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="7b819-132">See also</span></span>



- [<span data-ttu-id="7b819-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7b819-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

