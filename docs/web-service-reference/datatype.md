---
title: DataType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DataType
api_type:
- schema
ms.assetid: 267fe5aa-f9b1-4d4c-ac11-0f2e50ec2627
description: DataType 要素は、共有フォルダーによって共有されるデータの種類を表します。
ms.openlocfilehash: a7df8d38e10f0ab31038d790d8f35208d1be66d5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458832"
---
# <a name="datatype"></a><span data-ttu-id="6e3f6-103">DataType</span><span class="sxs-lookup"><span data-stu-id="6e3f6-103">DataType</span></span>

<span data-ttu-id="6e3f6-104">**DataType**要素は、共有フォルダーによって共有されるデータの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-104">The **DataType** element describes the type of data that is shared by a shared folder.</span></span> 
  
```xml
<DataType>Calendar or Contacts</DataType>
```

<span data-ttu-id="6e3f6-105">**SharingDataType**</span><span class="sxs-lookup"><span data-stu-id="6e3f6-105">**SharingDataType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6e3f6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6e3f6-106">Attributes and elements</span></span>

<span data-ttu-id="6e3f6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e3f6-108">属性</span><span class="sxs-lookup"><span data-stu-id="6e3f6-108">Attributes</span></span>

<span data-ttu-id="6e3f6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e3f6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6e3f6-110">Child elements</span></span>

<span data-ttu-id="6e3f6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6e3f6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6e3f6-112">Parent elements</span></span>

|<span data-ttu-id="6e3f6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6e3f6-113">**Element**</span></span>|<span data-ttu-id="6e3f6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6e3f6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e3f6-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="6e3f6-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="6e3f6-116">指定された共有フォルダーのローカルフォルダー識別子を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6e3f6-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6e3f6-117">Text value</span></span>

<span data-ttu-id="6e3f6-118">次の表に、 **DataType**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-118">The following table lists the possible values for the **DataType** element.</span></span> 
  
<span data-ttu-id="6e3f6-119">**DataType 要素の値**</span><span class="sxs-lookup"><span data-stu-id="6e3f6-119">**DataType element values**</span></span>

|<span data-ttu-id="6e3f6-120">**値**</span><span class="sxs-lookup"><span data-stu-id="6e3f6-120">**Value**</span></span>|<span data-ttu-id="6e3f6-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="6e3f6-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6e3f6-122">カレンダー</span><span class="sxs-lookup"><span data-stu-id="6e3f6-122">Calendar</span></span>  <br/> |<span data-ttu-id="6e3f6-123">共有フォルダーに予定表の情報が含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-123">Indicates that the shared folder contains calendar information.</span></span>  <br/> |
|<span data-ttu-id="6e3f6-124">連絡先</span><span class="sxs-lookup"><span data-stu-id="6e3f6-124">Contacts</span></span>  <br/> |<span data-ttu-id="6e3f6-125">共有フォルダーに連絡先情報が含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-125">Indicates that the shared folder contains contact information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6e3f6-126">注釈</span><span class="sxs-lookup"><span data-stu-id="6e3f6-126">Remarks</span></span>

<span data-ttu-id="6e3f6-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6e3f6-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e3f6-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6e3f6-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e3f6-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="6e3f6-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6e3f6-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6e3f6-130">Schema Name</span></span>  <br/> |<span data-ttu-id="6e3f6-131">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="6e3f6-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6e3f6-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6e3f6-132">Validation File</span></span>  <br/> |<span data-ttu-id="6e3f6-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6e3f6-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6e3f6-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6e3f6-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e3f6-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="6e3f6-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e3f6-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="6e3f6-136">See also</span></span>

- [<span data-ttu-id="6e3f6-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6e3f6-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

