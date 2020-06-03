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
description: UserConfigurationProperties 要素は、GetUserConfiguration 操作で取得するプロパティの種類を指定します。
ms.openlocfilehash: af6bee64516a7410d96ecc7581e8e819f550ddc1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466494"
---
# <a name="userconfigurationproperties"></a><span data-ttu-id="65b3a-103">UserConfigurationProperties</span><span class="sxs-lookup"><span data-stu-id="65b3a-103">UserConfigurationProperties</span></span>

<span data-ttu-id="65b3a-104">**Userconfigurationproperties**要素は、getuserconfiguration 操作で取得するプロパティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="65b3a-104">The **UserConfigurationProperties** element specifies the property types to get in a GetUserConfiguration operation.</span></span> 
  
```xml
<UserConfigurationProperties>Id | Dictionary | XmlData | BinaryData | All</UserConfigurationProperties>
```

 <span data-ttu-id="65b3a-105">**UserConfigurationPropertyType**</span><span class="sxs-lookup"><span data-stu-id="65b3a-105">**UserConfigurationPropertyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="65b3a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="65b3a-106">Attributes and elements</span></span>

<span data-ttu-id="65b3a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="65b3a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="65b3a-108">属性</span><span class="sxs-lookup"><span data-stu-id="65b3a-108">Attributes</span></span>

<span data-ttu-id="65b3a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="65b3a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="65b3a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="65b3a-110">Child elements</span></span>

<span data-ttu-id="65b3a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="65b3a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="65b3a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="65b3a-112">Parent elements</span></span>

|<span data-ttu-id="65b3a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="65b3a-113">**Element**</span></span>|<span data-ttu-id="65b3a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="65b3a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="65b3a-115">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="65b3a-115">GetUserConfiguration</span></span>](getuserconfiguration.md) <br/> |<span data-ttu-id="65b3a-116">ユーザー構成オブジェクトを取得する要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="65b3a-116">Specifies a request to get a user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="65b3a-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="65b3a-117">Text value</span></span>

<span data-ttu-id="65b3a-118">次の表に、 **Userconfigurationproperties**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="65b3a-118">The following table lists the possible values for the **UserConfigurationProperties** element.</span></span> 
  
|<span data-ttu-id="65b3a-119">**値**</span><span class="sxs-lookup"><span data-stu-id="65b3a-119">**Value**</span></span>|<span data-ttu-id="65b3a-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="65b3a-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="65b3a-121">ID</span><span class="sxs-lookup"><span data-stu-id="65b3a-121">Id</span></span>  <br/> |<span data-ttu-id="65b3a-122">Identifier プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="65b3a-122">Specifies the identifier property.</span></span>  <br/> |
|<span data-ttu-id="65b3a-123">Dictionary</span><span class="sxs-lookup"><span data-stu-id="65b3a-123">Dictionary</span></span>  <br/> |<span data-ttu-id="65b3a-124">ディクショナリのプロパティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="65b3a-124">Specifies dictionary property types.</span></span>  <br/> |
|<span data-ttu-id="65b3a-125">XmlData</span><span class="sxs-lookup"><span data-stu-id="65b3a-125">XmlData</span></span>  <br/> |<span data-ttu-id="65b3a-126">XML データプロパティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="65b3a-126">Specifies XML data property types.</span></span>  <br/> |
|<span data-ttu-id="65b3a-127">BinaryData</span><span class="sxs-lookup"><span data-stu-id="65b3a-127">BinaryData</span></span>  <br/> |<span data-ttu-id="65b3a-128">バイナリデータのプロパティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="65b3a-128">Specifies binary data property types.</span></span>  <br/> |
|<span data-ttu-id="65b3a-129">すべて</span><span class="sxs-lookup"><span data-stu-id="65b3a-129">All</span></span>  <br/> |<span data-ttu-id="65b3a-130">識別子、辞書、XML データ、およびバイナリデータのプロパティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="65b3a-130">Specifies the identifier, dictionary, XML data, and binary data property types.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="65b3a-131">注釈</span><span class="sxs-lookup"><span data-stu-id="65b3a-131">Remarks</span></span>

<span data-ttu-id="65b3a-132">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="65b3a-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="65b3a-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="65b3a-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="65b3a-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="65b3a-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="65b3a-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="65b3a-135">Schema Name</span></span>  <br/> |<span data-ttu-id="65b3a-136">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="65b3a-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="65b3a-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="65b3a-137">Validation File</span></span>  <br/> |<span data-ttu-id="65b3a-138">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="65b3a-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="65b3a-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="65b3a-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="65b3a-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="65b3a-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="65b3a-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="65b3a-141">See also</span></span>



- [<span data-ttu-id="65b3a-142">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="65b3a-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

