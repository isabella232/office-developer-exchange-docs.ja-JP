---
title: ExchangeStoreId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5acceb42-a757-4c74-ab1c-b1abf7bf1e0a
description: ExchangeStoreId 要素は、インスタントメッセージング (IM) グループ識別子を指定します。
ms.openlocfilehash: c1b1e1830987449eeb7ea186d00743ea9cc75a77
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456991"
---
# <a name="exchangestoreid"></a><span data-ttu-id="944a9-103">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="944a9-103">ExchangeStoreId</span></span>

<span data-ttu-id="944a9-104">**ExchangeStoreId**要素は、インスタントメッセージング (IM) グループ識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="944a9-104">The **ExchangeStoreId** element specifies the instant messaging (IM) group identifier.</span></span> 
  
```XML
<ExchangeStoreId Id="" ChangeKey=""/>
```

 <span data-ttu-id="944a9-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="944a9-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="944a9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="944a9-106">Attributes and elements</span></span>

<span data-ttu-id="944a9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="944a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="944a9-108">属性</span><span class="sxs-lookup"><span data-stu-id="944a9-108">Attributes</span></span>

|<span data-ttu-id="944a9-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="944a9-109">**Attribute**</span></span>|<span data-ttu-id="944a9-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="944a9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="944a9-111">ID</span><span class="sxs-lookup"><span data-stu-id="944a9-111">Id</span></span>  <br/> |<span data-ttu-id="944a9-112">**Id**属性のテキスト値は、グループの識別子です。</span><span class="sxs-lookup"><span data-stu-id="944a9-112">The text value of the **Id** attribute is the identifier of the group.</span></span>  <br/> |
|<span data-ttu-id="944a9-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="944a9-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="944a9-114">**Changekey**属性のテキスト値は、グループの変更キーです。</span><span class="sxs-lookup"><span data-stu-id="944a9-114">The text value of the **ChangeKey** attribute is the change key of the group.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="944a9-115">子要素</span><span class="sxs-lookup"><span data-stu-id="944a9-115">Child elements</span></span>

<span data-ttu-id="944a9-116">なし。</span><span class="sxs-lookup"><span data-stu-id="944a9-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="944a9-117">親要素</span><span class="sxs-lookup"><span data-stu-id="944a9-117">Parent elements</span></span>

|<span data-ttu-id="944a9-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="944a9-118">**Element**</span></span>|<span data-ttu-id="944a9-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="944a9-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="944a9-120">ImGroup</span><span class="sxs-lookup"><span data-stu-id="944a9-120">ImGroup</span></span>](imgroup.md) <br/> |<span data-ttu-id="944a9-121">インスタントメッセージンググループを表します。</span><span class="sxs-lookup"><span data-stu-id="944a9-121">Represents an instant messaging group.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="944a9-122">注釈</span><span class="sxs-lookup"><span data-stu-id="944a9-122">Remarks</span></span>

<span data-ttu-id="944a9-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="944a9-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="944a9-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="944a9-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="944a9-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="944a9-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="944a9-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="944a9-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="944a9-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="944a9-127">Schema Name</span></span>  <br/> |<span data-ttu-id="944a9-128">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="944a9-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="944a9-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="944a9-129">Validation File</span></span>  <br/> |<span data-ttu-id="944a9-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="944a9-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="944a9-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="944a9-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="944a9-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="944a9-132">See also</span></span>



- [<span data-ttu-id="944a9-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="944a9-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

