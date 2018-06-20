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
description: データ型の要素では、共有フォルダーが共有されているデータの種類について説明します。
ms.openlocfilehash: b1adac8e3029abd64df96ab1560706babe4b12f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759920"
---
# <a name="datatype"></a><span data-ttu-id="f9f75-103">DataType</span><span class="sxs-lookup"><span data-stu-id="f9f75-103">DataType</span></span>

<span data-ttu-id="f9f75-104">**データ型**の要素では、共有フォルダーが共有されているデータの種類について説明します。</span><span class="sxs-lookup"><span data-stu-id="f9f75-104">The **DataType** element describes the type of data that is shared by a shared folder.</span></span> 
  
```xml
<DataType>Calendar or Contacts</DataType>
```

<span data-ttu-id="f9f75-105">**SharingDataType**</span><span class="sxs-lookup"><span data-stu-id="f9f75-105">**SharingDataType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f9f75-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f9f75-106">Attributes and elements</span></span>

<span data-ttu-id="f9f75-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f9f75-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9f75-108">属性</span><span class="sxs-lookup"><span data-stu-id="f9f75-108">Attributes</span></span>

<span data-ttu-id="f9f75-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f9f75-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f9f75-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f9f75-110">Child elements</span></span>

<span data-ttu-id="f9f75-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f9f75-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f9f75-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f9f75-112">Parent elements</span></span>

|<span data-ttu-id="f9f75-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f9f75-113">**Element**</span></span>|<span data-ttu-id="f9f75-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f9f75-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9f75-115">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="f9f75-115">GetSharingFolder</span></span>](getsharingfolder.md) <br/> |<span data-ttu-id="f9f75-116">指定した共有フォルダーのローカル フォルダーの識別子を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="f9f75-116">Defines a request to get the local folder identifier of a specified shared folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f9f75-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f9f75-117">Text value</span></span>

<span data-ttu-id="f9f75-118">次の表は、**データ型**の要素の有効な値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="f9f75-118">The following table lists the possible values for the **DataType** element.</span></span> 
  
<span data-ttu-id="f9f75-119">**要素の値のデータ型**</span><span class="sxs-lookup"><span data-stu-id="f9f75-119">**DataType element values**</span></span>

|<span data-ttu-id="f9f75-120">**値**</span><span class="sxs-lookup"><span data-stu-id="f9f75-120">**Value**</span></span>|<span data-ttu-id="f9f75-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="f9f75-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f9f75-122">カレンダー</span><span class="sxs-lookup"><span data-stu-id="f9f75-122">Calendar</span></span>  <br/> |<span data-ttu-id="f9f75-123">共有フォルダーに、予定表の情報が含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="f9f75-123">Indicates that the shared folder contains calendar information.</span></span>  <br/> |
|<span data-ttu-id="f9f75-124">連絡先</span><span class="sxs-lookup"><span data-stu-id="f9f75-124">Contacts</span></span>  <br/> |<span data-ttu-id="f9f75-125">共有フォルダーに連絡先情報が含まれていることを示します。</span><span class="sxs-lookup"><span data-stu-id="f9f75-125">Indicates that the shared folder contains contact information.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f9f75-126">備考</span><span class="sxs-lookup"><span data-stu-id="f9f75-126">Remarks</span></span>

<span data-ttu-id="f9f75-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f9f75-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f9f75-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="f9f75-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9f75-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="f9f75-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f9f75-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f9f75-130">Schema Name</span></span>  <br/> |<span data-ttu-id="f9f75-131">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f9f75-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f9f75-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f9f75-132">Validation File</span></span>  <br/> |<span data-ttu-id="f9f75-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f9f75-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f9f75-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f9f75-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="f9f75-135">False</span><span class="sxs-lookup"><span data-stu-id="f9f75-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f9f75-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="f9f75-136">See also</span></span>

- [<span data-ttu-id="f9f75-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f9f75-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

