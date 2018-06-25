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
description: UserConfiguration 要素は、単一のユーザーの構成オブジェクトを定義します。
ms.openlocfilehash: ce3eaa470ef592c5a8e5a7ef24c377bb2feeca2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839925"
---
# <a name="userconfiguration"></a><span data-ttu-id="7c621-103">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c621-103">UserConfiguration</span></span>

<span data-ttu-id="7c621-104">**UserConfiguration**要素は、単一のユーザーの構成オブジェクトを定義します。</span><span class="sxs-lookup"><span data-stu-id="7c621-104">The **UserConfiguration** element defines a single user configuration object.</span></span> 
  
```XML
<UserConfiguration>
   <UserConfigurationName/>
   <ItemId/>
   <Dictionary/>
   <XmlData/>
  <BinaryData/>
</UserConfiguration>
```

 <span data-ttu-id="7c621-105">**UserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="7c621-105">**UserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c621-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7c621-106">Attributes and elements</span></span>

<span data-ttu-id="7c621-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7c621-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c621-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c621-108">Attributes</span></span>

<span data-ttu-id="7c621-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7c621-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c621-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7c621-110">Child elements</span></span>

|<span data-ttu-id="7c621-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="7c621-111">**Element**</span></span>|<span data-ttu-id="7c621-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c621-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c621-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="7c621-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="7c621-114">ユーザーの構成オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="7c621-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="7c621-115">ユーザーの構成オブジェクトを作成するとき、この要素を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c621-115">This element must be used when you create a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="7c621-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="7c621-116">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="7c621-117">ユーザー構成オブジェクトの項目の識別子を定義します。</span><span class="sxs-lookup"><span data-stu-id="7c621-117">Defines the user configuration object item identifier.</span></span>  <br/> |
|[<span data-ttu-id="7c621-118">辞書</span><span class="sxs-lookup"><span data-stu-id="7c621-118">Dictionary</span></span>](dictionary.md) <br/> |<span data-ttu-id="7c621-119">ユーザーの構成オブジェクトのディクショナリ プロパティのエントリのセットを定義します。</span><span class="sxs-lookup"><span data-stu-id="7c621-119">Defines a set of dictionary property entries for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="7c621-120">XmlData</span><span class="sxs-lookup"><span data-stu-id="7c621-120">XmlData</span></span>](xmldata.md) <br/> |<span data-ttu-id="7c621-121">ユーザーの構成オブジェクトの XML データのプロパティの内容が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7c621-121">Contains XML data property content for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="7c621-122">データ</span><span class="sxs-lookup"><span data-stu-id="7c621-122">BinaryData</span></span>](binarydata.md) <br/> |<span data-ttu-id="7c621-123">ユーザーの構成オブジェクトのバイナリ データ プロパティのコンテンツが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7c621-123">Contains binary data property content for a user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c621-124">親要素</span><span class="sxs-lookup"><span data-stu-id="7c621-124">Parent elements</span></span>

|<span data-ttu-id="7c621-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="7c621-125">**Element**</span></span>|<span data-ttu-id="7c621-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c621-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c621-127">CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c621-127">CreateUserConfiguration</span></span>](createuserconfiguration.md) <br/> |<span data-ttu-id="7c621-128">ユーザーの構成オブジェクトを作成する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="7c621-128">Represents a request to create a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="7c621-129">GetUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7c621-129">GetUserConfigurationResponseMessage</span></span>](getuserconfigurationresponsemessage.md) <br/> |<span data-ttu-id="7c621-130">ユーザーの構成オブジェクトを返す応答を表します。</span><span class="sxs-lookup"><span data-stu-id="7c621-130">Represents a response that returns a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="7c621-131">UpdateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c621-131">UpdateUserConfiguration</span></span>](updateuserconfiguration.md) <br/> |<span data-ttu-id="7c621-132">ユーザーの構成オブジェクトを更新する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="7c621-132">Represents a request to update a user configuration object.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c621-133">備考</span><span class="sxs-lookup"><span data-stu-id="7c621-133">Remarks</span></span>

<span data-ttu-id="7c621-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7c621-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c621-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="7c621-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c621-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="7c621-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7c621-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7c621-137">Schema Name</span></span>  <br/> |<span data-ttu-id="7c621-138">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7c621-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7c621-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7c621-139">Validation File</span></span>  <br/> |<span data-ttu-id="7c621-140">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7c621-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7c621-141">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7c621-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c621-142">False</span><span class="sxs-lookup"><span data-stu-id="7c621-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c621-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="7c621-143">See also</span></span>



- [<span data-ttu-id="7c621-144">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7c621-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

