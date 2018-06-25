---
title: UserConfigurationProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationProperties
api_type:
- schema
ms.assetid: c143a6ec-62ad-4d48-b844-b1ad88054bc1
description: UserConfigurationProperties 要素は、GetUserConfiguration の操作で取得するプロパティの型を指定します。
ms.openlocfilehash: 4f993765bb7c36f28a41a3f2fa7e28698a3f709e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839928"
---
# <a name="userconfigurationproperties"></a><span data-ttu-id="27aff-103">UserConfigurationProperties</span><span class="sxs-lookup"><span data-stu-id="27aff-103">UserConfigurationProperties</span></span>

<span data-ttu-id="27aff-104">**UserConfigurationProperties**要素は、GetUserConfiguration の操作で取得するプロパティの型を指定します。</span><span class="sxs-lookup"><span data-stu-id="27aff-104">The **UserConfigurationProperties** element specifies the property types to get in a GetUserConfiguration operation.</span></span> 
  
```xml
<UserConfigurationProperties>Id | Dictionary | XmlData | BinaryData | All</UserConfigurationProperties>
```

 <span data-ttu-id="27aff-105">**UserConfigurationPropertyType**</span><span class="sxs-lookup"><span data-stu-id="27aff-105">**UserConfigurationPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="27aff-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="27aff-106">Attributes and elements</span></span>

<span data-ttu-id="27aff-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="27aff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="27aff-108">属性</span><span class="sxs-lookup"><span data-stu-id="27aff-108">Attributes</span></span>

<span data-ttu-id="27aff-109">なし。</span><span class="sxs-lookup"><span data-stu-id="27aff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="27aff-110">子要素</span><span class="sxs-lookup"><span data-stu-id="27aff-110">Child elements</span></span>

<span data-ttu-id="27aff-111">なし。</span><span class="sxs-lookup"><span data-stu-id="27aff-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="27aff-112">親要素</span><span class="sxs-lookup"><span data-stu-id="27aff-112">Parent elements</span></span>

|<span data-ttu-id="27aff-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="27aff-113">**Element**</span></span>|<span data-ttu-id="27aff-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="27aff-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="27aff-115">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="27aff-115">GetUserConfiguration</span></span>](getuserconfiguration.md) <br/> |<span data-ttu-id="27aff-116">ユーザーの構成オブジェクトを取得する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="27aff-116">Specifies a request to get a user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="27aff-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="27aff-117">Text value</span></span>

<span data-ttu-id="27aff-118">次の表は、 **UserConfigurationProperties**要素の値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="27aff-118">The following table lists the possible values for the **UserConfigurationProperties** element.</span></span> 
  
|<span data-ttu-id="27aff-119">**値**</span><span class="sxs-lookup"><span data-stu-id="27aff-119">**Value**</span></span>|<span data-ttu-id="27aff-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="27aff-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="27aff-121">ID</span><span class="sxs-lookup"><span data-stu-id="27aff-121">Id</span></span>  <br/> |<span data-ttu-id="27aff-122">識別子のプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="27aff-122">Specifies the identifier property.</span></span>  <br/> |
|<span data-ttu-id="27aff-123">Dictionary</span><span class="sxs-lookup"><span data-stu-id="27aff-123">Dictionary</span></span>  <br/> |<span data-ttu-id="27aff-124">ディクショナリ プロパティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="27aff-124">Specifies dictionary property types.</span></span>  <br/> |
|<span data-ttu-id="27aff-125">XmlData</span><span class="sxs-lookup"><span data-stu-id="27aff-125">XmlData</span></span>  <br/> |<span data-ttu-id="27aff-126">プロパティの XML データ型を指定します。</span><span class="sxs-lookup"><span data-stu-id="27aff-126">Specifies XML data property types.</span></span>  <br/> |
|<span data-ttu-id="27aff-127">データ</span><span class="sxs-lookup"><span data-stu-id="27aff-127">BinaryData</span></span>  <br/> |<span data-ttu-id="27aff-128">バイナリ データのプロパティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="27aff-128">Specifies binary data property types.</span></span>  <br/> |
|<span data-ttu-id="27aff-129">All</span><span class="sxs-lookup"><span data-stu-id="27aff-129">All</span></span>  <br/> |<span data-ttu-id="27aff-130">識別子、ディクショナリ、XML データ、およびバイナリ データのプロパティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="27aff-130">Specifies the identifier, dictionary, XML data, and binary data property types.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="27aff-131">備考</span><span class="sxs-lookup"><span data-stu-id="27aff-131">Remarks</span></span>

<span data-ttu-id="27aff-132">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="27aff-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="27aff-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="27aff-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="27aff-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="27aff-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="27aff-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="27aff-135">Schema Name</span></span>  <br/> |<span data-ttu-id="27aff-136">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="27aff-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="27aff-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="27aff-137">Validation File</span></span>  <br/> |<span data-ttu-id="27aff-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="27aff-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="27aff-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="27aff-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="27aff-140">False</span><span class="sxs-lookup"><span data-stu-id="27aff-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="27aff-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="27aff-141">See also</span></span>



- [<span data-ttu-id="27aff-142">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="27aff-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

