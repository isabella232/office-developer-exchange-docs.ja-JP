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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457712"
---
# <a name="getuserconfiguration"></a><span data-ttu-id="4bf99-103">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="4bf99-103">GetUserConfiguration</span></span>

<span data-ttu-id="4bf99-104">**Getuserconfiguration**要素は、ユーザー構成オブジェクトを取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="4bf99-104">The **GetUserConfiguration** element represent a request to get a user configuration object.</span></span> 
  
```XML
<GetUserConfiguration>
   <UserConfigurationName/>
   <UserConfigurationProperties/>
</GetUserConfiguration>
```

 <span data-ttu-id="4bf99-105">**GetUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="4bf99-105">**GetUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4bf99-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4bf99-106">Attributes and elements</span></span>

<span data-ttu-id="4bf99-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4bf99-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4bf99-108">属性</span><span class="sxs-lookup"><span data-stu-id="4bf99-108">Attributes</span></span>

<span data-ttu-id="4bf99-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4bf99-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4bf99-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4bf99-110">Child elements</span></span>

|<span data-ttu-id="4bf99-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="4bf99-111">**Element**</span></span>|<span data-ttu-id="4bf99-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4bf99-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4bf99-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="4bf99-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="4bf99-114">ユーザー構成オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="4bf99-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="4bf99-115">この要素は、GetUserConfiguration 要求に存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4bf99-115">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
|[<span data-ttu-id="4bf99-116">UserConfigurationProperties</span><span class="sxs-lookup"><span data-stu-id="4bf99-116">UserConfigurationProperties</span></span>](userconfigurationproperties.md) <br/> |<span data-ttu-id="4bf99-117">返すユーザー構成プロパティの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="4bf99-117">Specifies the user configuration property types to return.</span></span> <span data-ttu-id="4bf99-118">この要素は、GetUserConfiguration 要求に存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4bf99-118">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4bf99-119">親要素</span><span class="sxs-lookup"><span data-stu-id="4bf99-119">Parent elements</span></span>

<span data-ttu-id="4bf99-120">なし。</span><span class="sxs-lookup"><span data-stu-id="4bf99-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="4bf99-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4bf99-121">Text value</span></span>

<span data-ttu-id="4bf99-122">なし。</span><span class="sxs-lookup"><span data-stu-id="4bf99-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4bf99-123">注釈</span><span class="sxs-lookup"><span data-stu-id="4bf99-123">Remarks</span></span>

<span data-ttu-id="4bf99-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4bf99-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4bf99-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4bf99-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4bf99-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="4bf99-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4bf99-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4bf99-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4bf99-128">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="4bf99-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4bf99-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4bf99-129">Validation File</span></span>  <br/> |<span data-ttu-id="4bf99-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4bf99-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4bf99-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4bf99-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="4bf99-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="4bf99-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4bf99-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="4bf99-133">See also</span></span>



- [<span data-ttu-id="4bf99-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4bf99-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

