---
title: UserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfiguration
api_type:
- schema
ms.assetid: 1811df99-ca5b-48a3-b160-b3fd70320c34
description: UserConfiguration 要素は、1つのユーザー構成オブジェクトを定義します。
ms.openlocfilehash: 1217f5d591570c2d8df49a116b6bf35c243d1e0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468909"
---
# <a name="userconfiguration"></a><span data-ttu-id="c352d-103">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="c352d-103">UserConfiguration</span></span>

<span data-ttu-id="c352d-104">**Userconfiguration**要素は、1つのユーザー構成オブジェクトを定義します。</span><span class="sxs-lookup"><span data-stu-id="c352d-104">The **UserConfiguration** element defines a single user configuration object.</span></span> 
  
```XML
<UserConfiguration>
   <UserConfigurationName/>
   <ItemId/>
   <Dictionary/>
   <XmlData/>
  <BinaryData/>
</UserConfiguration>
```

 <span data-ttu-id="c352d-105">**UserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="c352d-105">**UserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c352d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c352d-106">Attributes and elements</span></span>

<span data-ttu-id="c352d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c352d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c352d-108">属性</span><span class="sxs-lookup"><span data-stu-id="c352d-108">Attributes</span></span>

<span data-ttu-id="c352d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c352d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c352d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c352d-110">Child elements</span></span>

|<span data-ttu-id="c352d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="c352d-111">**Element**</span></span>|<span data-ttu-id="c352d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="c352d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c352d-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="c352d-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="c352d-114">ユーザー構成オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="c352d-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="c352d-115">この要素は、ユーザー構成オブジェクトを作成するときに使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c352d-115">This element must be used when you create a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="c352d-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="c352d-116">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="c352d-117">ユーザー構成オブジェクトのアイテム識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="c352d-117">Defines the user configuration object item identifier.</span></span>  <br/> |
|[<span data-ttu-id="c352d-118">辞書</span><span class="sxs-lookup"><span data-stu-id="c352d-118">Dictionary</span></span>](dictionary.md) <br/> |<span data-ttu-id="c352d-119">ユーザー構成オブジェクトの辞書のプロパティエントリのセットを定義します。</span><span class="sxs-lookup"><span data-stu-id="c352d-119">Defines a set of dictionary property entries for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="c352d-120">XmlData</span><span class="sxs-lookup"><span data-stu-id="c352d-120">XmlData</span></span>](xmldata.md) <br/> |<span data-ttu-id="c352d-121">ユーザー構成オブジェクトの XML データプロパティコンテンツが保存されています。</span><span class="sxs-lookup"><span data-stu-id="c352d-121">Contains XML data property content for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="c352d-122">BinaryData</span><span class="sxs-lookup"><span data-stu-id="c352d-122">BinaryData</span></span>](binarydata.md) <br/> |<span data-ttu-id="c352d-123">ユーザー構成オブジェクトのバイナリデータのプロパティコンテンツが保存されています。</span><span class="sxs-lookup"><span data-stu-id="c352d-123">Contains binary data property content for a user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c352d-124">親要素</span><span class="sxs-lookup"><span data-stu-id="c352d-124">Parent elements</span></span>

|<span data-ttu-id="c352d-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="c352d-125">**Element**</span></span>|<span data-ttu-id="c352d-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="c352d-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c352d-127">CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="c352d-127">CreateUserConfiguration</span></span>](createuserconfiguration.md) <br/> |<span data-ttu-id="c352d-128">ユーザー構成オブジェクトを作成するための要求を表します。</span><span class="sxs-lookup"><span data-stu-id="c352d-128">Represents a request to create a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="c352d-129">GetUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c352d-129">GetUserConfigurationResponseMessage</span></span>](getuserconfigurationresponsemessage.md) <br/> |<span data-ttu-id="c352d-130">ユーザー構成オブジェクトを返す応答を表します。</span><span class="sxs-lookup"><span data-stu-id="c352d-130">Represents a response that returns a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="c352d-131">UpdateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="c352d-131">UpdateUserConfiguration</span></span>](updateuserconfiguration.md) <br/> |<span data-ttu-id="c352d-132">ユーザー構成オブジェクトを更新する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="c352d-132">Represents a request to update a user configuration object.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c352d-133">注釈</span><span class="sxs-lookup"><span data-stu-id="c352d-133">Remarks</span></span>

<span data-ttu-id="c352d-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c352d-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c352d-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c352d-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c352d-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="c352d-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c352d-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c352d-137">Schema Name</span></span>  <br/> |<span data-ttu-id="c352d-138">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c352d-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c352d-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c352d-139">Validation File</span></span>  <br/> |<span data-ttu-id="c352d-140">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c352d-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c352d-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c352d-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="c352d-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="c352d-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c352d-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="c352d-143">See also</span></span>



- [<span data-ttu-id="c352d-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c352d-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

