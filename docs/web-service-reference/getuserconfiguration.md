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
description: GetUserConfiguration 要素は、ユーザーの構成オブジェクトを取得する要求を表します。
ms.openlocfilehash: 81f2ca4995de69d6547412ec699a2ceaddcce385
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831688"
---
# <a name="getuserconfiguration"></a><span data-ttu-id="540e0-103">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="540e0-103">GetUserConfiguration</span></span>

<span data-ttu-id="540e0-104">**GetUserConfiguration**要素は、ユーザーの構成オブジェクトを取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="540e0-104">The **GetUserConfiguration** element represent a request to get a user configuration object.</span></span> 
  
```XML
<GetUserConfiguration>
   <UserConfigurationName/>
   <UserConfigurationProperties/>
</GetUserConfiguration>
```

 <span data-ttu-id="540e0-105">**GetUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="540e0-105">**GetUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="540e0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="540e0-106">Attributes and elements</span></span>

<span data-ttu-id="540e0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="540e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="540e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="540e0-108">Attributes</span></span>

<span data-ttu-id="540e0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="540e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="540e0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="540e0-110">Child elements</span></span>

|<span data-ttu-id="540e0-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="540e0-111">**Element**</span></span>|<span data-ttu-id="540e0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="540e0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="540e0-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="540e0-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="540e0-114">ユーザーの構成オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="540e0-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="540e0-115">この要素は、GetUserConfiguration 要求内に存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="540e0-115">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
|[<span data-ttu-id="540e0-116">UserConfigurationProperties</span><span class="sxs-lookup"><span data-stu-id="540e0-116">UserConfigurationProperties</span></span>](userconfigurationproperties.md) <br/> |<span data-ttu-id="540e0-117">取得するユーザーの構成プロパティの型を指定します。</span><span class="sxs-lookup"><span data-stu-id="540e0-117">Specifies the user configuration property types to return.</span></span> <span data-ttu-id="540e0-118">この要素は、GetUserConfiguration 要求内に存在する必要があります。</span><span class="sxs-lookup"><span data-stu-id="540e0-118">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="540e0-119">親要素</span><span class="sxs-lookup"><span data-stu-id="540e0-119">Parent elements</span></span>

<span data-ttu-id="540e0-120">なし。</span><span class="sxs-lookup"><span data-stu-id="540e0-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="540e0-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="540e0-121">Text value</span></span>

<span data-ttu-id="540e0-122">なし。</span><span class="sxs-lookup"><span data-stu-id="540e0-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="540e0-123">備考</span><span class="sxs-lookup"><span data-stu-id="540e0-123">Remarks</span></span>

<span data-ttu-id="540e0-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="540e0-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="540e0-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="540e0-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="540e0-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="540e0-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="540e0-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="540e0-127">Schema Name</span></span>  <br/> |<span data-ttu-id="540e0-128">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="540e0-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="540e0-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="540e0-129">Validation File</span></span>  <br/> |<span data-ttu-id="540e0-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="540e0-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="540e0-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="540e0-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="540e0-132">False</span><span class="sxs-lookup"><span data-stu-id="540e0-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="540e0-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="540e0-133">See also</span></span>



- [<span data-ttu-id="540e0-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="540e0-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

