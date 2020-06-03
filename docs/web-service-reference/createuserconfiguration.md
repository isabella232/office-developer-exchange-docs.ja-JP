---
title: CreateUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateUserConfiguration
api_type:
- schema
ms.assetid: 43e12e8b-5629-4f5f-9cbd-a99084d8460f
description: CreateUserConfiguration 要素は、ユーザー構成オブジェクトを作成する要求を表します。
ms.openlocfilehash: 1d9194baf309936cb4be088a7ff56250dfa349cc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463777"
---
# <a name="createuserconfiguration"></a><span data-ttu-id="bd5ba-103">CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd5ba-103">CreateUserConfiguration</span></span>

<span data-ttu-id="bd5ba-104">**CreateUserConfiguration**要素は、ユーザー構成オブジェクトを作成する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="bd5ba-104">The **CreateUserConfiguration** element represents a request to create a user configuration object.</span></span> 
  
```xml
<CreateUserConfiguration>
   <UserConfiguration/>
</CreateUserConfiguration>
```

 <span data-ttu-id="bd5ba-105">**CreateUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="bd5ba-105">**CreateUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd5ba-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="bd5ba-106">Attributes and elements</span></span>

<span data-ttu-id="bd5ba-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bd5ba-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd5ba-108">属性</span><span class="sxs-lookup"><span data-stu-id="bd5ba-108">Attributes</span></span>

<span data-ttu-id="bd5ba-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bd5ba-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd5ba-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bd5ba-110">Child elements</span></span>

|<span data-ttu-id="bd5ba-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="bd5ba-111">**Element**</span></span>|<span data-ttu-id="bd5ba-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="bd5ba-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd5ba-113">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd5ba-113">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="bd5ba-114">1つのユーザー構成オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="bd5ba-114">Represents a single user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd5ba-115">親要素</span><span class="sxs-lookup"><span data-stu-id="bd5ba-115">Parent elements</span></span>

<span data-ttu-id="bd5ba-116">なし。</span><span class="sxs-lookup"><span data-stu-id="bd5ba-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="bd5ba-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bd5ba-117">Text value</span></span>

<span data-ttu-id="bd5ba-118">なし。</span><span class="sxs-lookup"><span data-stu-id="bd5ba-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bd5ba-119">注釈</span><span class="sxs-lookup"><span data-stu-id="bd5ba-119">Remarks</span></span>

<span data-ttu-id="bd5ba-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="bd5ba-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd5ba-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="bd5ba-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd5ba-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="bd5ba-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bd5ba-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bd5ba-123">Schema Name</span></span>  <br/> |<span data-ttu-id="bd5ba-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="bd5ba-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bd5ba-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bd5ba-125">Validation File</span></span>  <br/> |<span data-ttu-id="bd5ba-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="bd5ba-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bd5ba-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bd5ba-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="bd5ba-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="bd5ba-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd5ba-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="bd5ba-129">See also</span></span>



- [<span data-ttu-id="bd5ba-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="bd5ba-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

