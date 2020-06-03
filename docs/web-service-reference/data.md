---
title: データ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Data
api_type:
- schema
ms.assetid: f875e6c2-be18-439a-a7b1-bb49a149b538
description: Data 要素には、共有データを表す暗号化されたデータが含まれています。
ms.openlocfilehash: cd13d68afcd0f40486865887676d2b5669c276f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529218"
---
# <a name="data"></a><span data-ttu-id="2402c-103">データ</span><span class="sxs-lookup"><span data-stu-id="2402c-103">Data</span></span>

<span data-ttu-id="2402c-104">**Data**要素には、共有データを表す暗号化されたデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2402c-104">The **Data** element contains encrypted data that represents the shared data.</span></span> 
  
- [<span data-ttu-id="2402c-105">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="2402c-105">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md)  
- [<span data-ttu-id="2402c-106">Data</span><span class="sxs-lookup"><span data-stu-id="2402c-106">Data</span></span>](data.md)
  
```xml
<Data/>
```

<span data-ttu-id="2402c-107">**EncryptedDataContainerType**</span><span class="sxs-lookup"><span data-stu-id="2402c-107">**EncryptedDataContainerType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2402c-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2402c-108">Attributes and elements</span></span>

<span data-ttu-id="2402c-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2402c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2402c-110">属性</span><span class="sxs-lookup"><span data-stu-id="2402c-110">Attributes</span></span>

<span data-ttu-id="2402c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2402c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2402c-112">子要素</span><span class="sxs-lookup"><span data-stu-id="2402c-112">Child elements</span></span>

<span data-ttu-id="2402c-113">なし。</span><span class="sxs-lookup"><span data-stu-id="2402c-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2402c-114">親要素</span><span class="sxs-lookup"><span data-stu-id="2402c-114">Parent elements</span></span>

|<span data-ttu-id="2402c-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="2402c-115">**Element**</span></span>|<span data-ttu-id="2402c-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="2402c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2402c-117">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="2402c-117">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="2402c-118">クライアントが他のクライアントと予定表または連絡先データの共有を承認するために使用できる暗号化されたデータを格納します。</span><span class="sxs-lookup"><span data-stu-id="2402c-118">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2402c-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2402c-119">Text value</span></span>

<span data-ttu-id="2402c-120">なし。</span><span class="sxs-lookup"><span data-stu-id="2402c-120">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2402c-121">注釈</span><span class="sxs-lookup"><span data-stu-id="2402c-121">Remarks</span></span>

<span data-ttu-id="2402c-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2402c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2402c-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2402c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2402c-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="2402c-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2402c-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2402c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2402c-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="2402c-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="2402c-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2402c-127">Validation File</span></span>  <br/> |<span data-ttu-id="2402c-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="2402c-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2402c-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2402c-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="2402c-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="2402c-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2402c-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="2402c-131">See also</span></span>

- [<span data-ttu-id="2402c-132">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="2402c-132">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="2402c-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2402c-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

