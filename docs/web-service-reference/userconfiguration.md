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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468909"
---
# <a name="userconfiguration"></a><span data-ttu-id="eeccc-103">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="eeccc-103">UserConfiguration</span></span>

<span data-ttu-id="eeccc-104">**Userconfiguration**要素は、1つのユーザー構成オブジェクトを定義します。</span><span class="sxs-lookup"><span data-stu-id="eeccc-104">The **UserConfiguration** element defines a single user configuration object.</span></span> 
  
```XML
<UserConfiguration>
   <UserConfigurationName/>
   <ItemId/>
   <Dictionary/>
   <XmlData/>
  <BinaryData/>
</UserConfiguration>
```

 <span data-ttu-id="eeccc-105">**UserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="eeccc-105">**UserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eeccc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="eeccc-106">Attributes and elements</span></span>

<span data-ttu-id="eeccc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="eeccc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eeccc-108">属性</span><span class="sxs-lookup"><span data-stu-id="eeccc-108">Attributes</span></span>

<span data-ttu-id="eeccc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="eeccc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eeccc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="eeccc-110">Child elements</span></span>

|<span data-ttu-id="eeccc-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="eeccc-111">**Element**</span></span>|<span data-ttu-id="eeccc-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="eeccc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eeccc-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="eeccc-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="eeccc-114">ユーザー構成オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="eeccc-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="eeccc-115">この要素は、ユーザー構成オブジェクトを作成するときに使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="eeccc-115">This element must be used when you create a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="eeccc-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="eeccc-116">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="eeccc-117">ユーザー構成オブジェクトのアイテム識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="eeccc-117">Defines the user configuration object item identifier.</span></span>  <br/> |
|[<span data-ttu-id="eeccc-118">辞書</span><span class="sxs-lookup"><span data-stu-id="eeccc-118">Dictionary</span></span>](dictionary.md) <br/> |<span data-ttu-id="eeccc-119">ユーザー構成オブジェクトの辞書のプロパティエントリのセットを定義します。</span><span class="sxs-lookup"><span data-stu-id="eeccc-119">Defines a set of dictionary property entries for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="eeccc-120">XmlData</span><span class="sxs-lookup"><span data-stu-id="eeccc-120">XmlData</span></span>](xmldata.md) <br/> |<span data-ttu-id="eeccc-121">ユーザー構成オブジェクトの XML データプロパティコンテンツが保存されています。</span><span class="sxs-lookup"><span data-stu-id="eeccc-121">Contains XML data property content for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="eeccc-122">BinaryData</span><span class="sxs-lookup"><span data-stu-id="eeccc-122">BinaryData</span></span>](binarydata.md) <br/> |<span data-ttu-id="eeccc-123">ユーザー構成オブジェクトのバイナリデータのプロパティコンテンツが保存されています。</span><span class="sxs-lookup"><span data-stu-id="eeccc-123">Contains binary data property content for a user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eeccc-124">親要素</span><span class="sxs-lookup"><span data-stu-id="eeccc-124">Parent elements</span></span>

|<span data-ttu-id="eeccc-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="eeccc-125">**Element**</span></span>|<span data-ttu-id="eeccc-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="eeccc-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eeccc-127">CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="eeccc-127">CreateUserConfiguration</span></span>](createuserconfiguration.md) <br/> |<span data-ttu-id="eeccc-128">ユーザー構成オブジェクトを作成するための要求を表します。</span><span class="sxs-lookup"><span data-stu-id="eeccc-128">Represents a request to create a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="eeccc-129">GetUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="eeccc-129">GetUserConfigurationResponseMessage</span></span>](getuserconfigurationresponsemessage.md) <br/> |<span data-ttu-id="eeccc-130">ユーザー構成オブジェクトを返す応答を表します。</span><span class="sxs-lookup"><span data-stu-id="eeccc-130">Represents a response that returns a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="eeccc-131">UpdateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="eeccc-131">UpdateUserConfiguration</span></span>](updateuserconfiguration.md) <br/> |<span data-ttu-id="eeccc-132">ユーザー構成オブジェクトを更新する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="eeccc-132">Represents a request to update a user configuration object.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eeccc-133">注釈</span><span class="sxs-lookup"><span data-stu-id="eeccc-133">Remarks</span></span>

<span data-ttu-id="eeccc-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="eeccc-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eeccc-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="eeccc-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eeccc-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="eeccc-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="eeccc-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="eeccc-137">Schema Name</span></span>  <br/> |<span data-ttu-id="eeccc-138">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="eeccc-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="eeccc-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="eeccc-139">Validation File</span></span>  <br/> |<span data-ttu-id="eeccc-140">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="eeccc-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eeccc-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="eeccc-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="eeccc-142">正しくない</span><span class="sxs-lookup"><span data-stu-id="eeccc-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eeccc-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="eeccc-143">See also</span></span>



- [<span data-ttu-id="eeccc-144">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="eeccc-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

