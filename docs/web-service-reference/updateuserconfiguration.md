---
title: UpdateUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateUserConfiguration
api_type:
- schema
ms.assetid: ccf7c577-f882-477e-9f6f-2f56729f7d77
description: UpdateUserConfiguration 要素は、ユーザー構成オブジェクトを更新する要求を表します。
ms.openlocfilehash: b46552dc93523340b04f4abfb07dc4fca7dd7898
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468832"
---
# <a name="updateuserconfiguration"></a><span data-ttu-id="74114-103">UpdateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="74114-103">UpdateUserConfiguration</span></span>

<span data-ttu-id="74114-104">**Updateuserconfiguration**要素は、ユーザー構成オブジェクトを更新する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="74114-104">The **UpdateUserConfiguration** element represents a request to update a user configuration object.</span></span> 
  
```XML
<UpdateUserConfiguration>
   <UserConfiguration/>
</UpdateUserConfiguration>
```

 <span data-ttu-id="74114-105">**UpdateUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="74114-105">**UpdateUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74114-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="74114-106">Attributes and elements</span></span>

<span data-ttu-id="74114-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="74114-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74114-108">属性</span><span class="sxs-lookup"><span data-stu-id="74114-108">Attributes</span></span>

<span data-ttu-id="74114-109">なし。</span><span class="sxs-lookup"><span data-stu-id="74114-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="74114-110">子要素</span><span class="sxs-lookup"><span data-stu-id="74114-110">Child elements</span></span>

|<span data-ttu-id="74114-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="74114-111">**Element**</span></span>|<span data-ttu-id="74114-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="74114-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74114-113">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="74114-113">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="74114-114">1つのユーザー構成オブジェクトを定義します。</span><span class="sxs-lookup"><span data-stu-id="74114-114">Defines a single user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74114-115">親要素</span><span class="sxs-lookup"><span data-stu-id="74114-115">Parent elements</span></span>

<span data-ttu-id="74114-116">なし。</span><span class="sxs-lookup"><span data-stu-id="74114-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="74114-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="74114-117">Text value</span></span>

<span data-ttu-id="74114-118">なし。</span><span class="sxs-lookup"><span data-stu-id="74114-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="74114-119">注釈</span><span class="sxs-lookup"><span data-stu-id="74114-119">Remarks</span></span>

<span data-ttu-id="74114-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="74114-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74114-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="74114-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74114-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="74114-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="74114-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="74114-123">Schema Name</span></span>  <br/> |<span data-ttu-id="74114-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="74114-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="74114-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="74114-125">Validation File</span></span>  <br/> |<span data-ttu-id="74114-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="74114-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74114-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="74114-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="74114-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="74114-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74114-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="74114-129">See also</span></span>



- [<span data-ttu-id="74114-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="74114-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

