---
title: GetUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserConfiguration
api_type:
- schema
ms.assetid: 4044c0a1-cd88-41ae-9cc4-a7cf2b279094
description: GetUserConfiguration 要素は、ユーザー構成オブジェクトを取得する要求を表します。
ms.openlocfilehash: 46a2a5ebbabfc038692a5de83e0a960e05295061
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457712"
---
# <a name="getuserconfiguration"></a><span data-ttu-id="b445d-103">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="b445d-103">GetUserConfiguration</span></span>

<span data-ttu-id="b445d-104">**Getuserconfiguration**要素は、ユーザー構成オブジェクトを取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="b445d-104">The **GetUserConfiguration** element represent a request to get a user configuration object.</span></span> 
  
```XML
<GetUserConfiguration>
   <UserConfigurationName/>
   <UserConfigurationProperties/>
</GetUserConfiguration>
```

 <span data-ttu-id="b445d-105">**GetUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="b445d-105">**GetUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b445d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b445d-106">Attributes and elements</span></span>

<span data-ttu-id="b445d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b445d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b445d-108">属性</span><span class="sxs-lookup"><span data-stu-id="b445d-108">Attributes</span></span>

<span data-ttu-id="b445d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b445d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b445d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b445d-110">Child elements</span></span>

|<span data-ttu-id="b445d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="b445d-111">**Element**</span></span>|<span data-ttu-id="b445d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b445d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b445d-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="b445d-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="b445d-114">ユーザー構成オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="b445d-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="b445d-115">この要素は、GetUserConfiguration 要求に存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b445d-115">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
|[<span data-ttu-id="b445d-116">UserConfigurationProperties</span><span class="sxs-lookup"><span data-stu-id="b445d-116">UserConfigurationProperties</span></span>](userconfigurationproperties.md) <br/> |<span data-ttu-id="b445d-117">返すユーザー構成プロパティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="b445d-117">Specifies the user configuration property types to return.</span></span> <span data-ttu-id="b445d-118">この要素は、GetUserConfiguration 要求に存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b445d-118">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b445d-119">親要素</span><span class="sxs-lookup"><span data-stu-id="b445d-119">Parent elements</span></span>

<span data-ttu-id="b445d-120">なし。</span><span class="sxs-lookup"><span data-stu-id="b445d-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b445d-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b445d-121">Text value</span></span>

<span data-ttu-id="b445d-122">なし。</span><span class="sxs-lookup"><span data-stu-id="b445d-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b445d-123">注釈</span><span class="sxs-lookup"><span data-stu-id="b445d-123">Remarks</span></span>

<span data-ttu-id="b445d-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b445d-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b445d-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b445d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b445d-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="b445d-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b445d-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b445d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="b445d-128">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b445d-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b445d-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b445d-129">Validation File</span></span>  <br/> |<span data-ttu-id="b445d-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b445d-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b445d-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b445d-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="b445d-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="b445d-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b445d-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="b445d-133">See also</span></span>



- [<span data-ttu-id="b445d-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b445d-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

