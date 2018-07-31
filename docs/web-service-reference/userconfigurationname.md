---
title: UserConfigurationName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationName
api_type:
- schema
ms.assetid: 6947dd03-9727-4379-9b9d-42373fa120c7
description: UserConfigurationName 要素は、ユーザーの構成オブジェクトの名前を表します。 ユーザーの構成オブジェクトの名前は、ユーザーの構成オブジェクトの識別子です。
ms.openlocfilehash: 33b3fc316a06b8088eb20a71788a9e6a3394d0d4
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354303"
---
# <a name="userconfigurationname"></a><span data-ttu-id="7c416-104">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="7c416-104">UserConfigurationName</span></span>

<span data-ttu-id="7c416-105">**UserConfigurationName**要素は、ユーザーの構成オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="7c416-105">The **UserConfigurationName** element represents the name of a user configuration object.</span></span> <span data-ttu-id="7c416-106">ユーザーの構成オブジェクトの名前は、ユーザーの構成オブジェクトの識別子です。</span><span class="sxs-lookup"><span data-stu-id="7c416-106">The user configuration object name is the identifier for a user configuration object.</span></span> 
  
```XML
<UserConfigurationName Name="">
   <FolderId/>
</UserConfigurationName>
```

```XML
<UserConfigurationName Name="">
   <DistinguishedFolderId/> 
</UserConfigurationName>
```

<span data-ttu-id="7c416-107">**UserConfigurationNameType**</span><span class="sxs-lookup"><span data-stu-id="7c416-107">**UserConfigurationNameType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7c416-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7c416-108">Attributes and elements</span></span>

<span data-ttu-id="7c416-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7c416-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c416-110">属性</span><span class="sxs-lookup"><span data-stu-id="7c416-110">Attributes</span></span>

|<span data-ttu-id="7c416-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="7c416-111">**Attribute**</span></span>|<span data-ttu-id="7c416-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c416-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7c416-113">**名前**</span><span class="sxs-lookup"><span data-stu-id="7c416-113">**Name**</span></span> <br/> |<span data-ttu-id="7c416-114">ユーザーの構成オブジェクトの名前を表す文字列値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7c416-114">Contains a string value that represents the name of a user configuration object.</span></span> <span data-ttu-id="7c416-115">この属性は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c416-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7c416-116">子要素</span><span class="sxs-lookup"><span data-stu-id="7c416-116">Child elements</span></span>

|<span data-ttu-id="7c416-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="7c416-117">**Element**</span></span>|<span data-ttu-id="7c416-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c416-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c416-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="7c416-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="7c416-120">ユーザーの構成オブジェクトが含まれているフォルダーのフォルダー id を表します。</span><span class="sxs-lookup"><span data-stu-id="7c416-120">Represents the folder identifier of the folder that contains the user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="7c416-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="7c416-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="7c416-122">ユーザーの構成オブジェクトが含まれているフォルダーの識別フォルダー名を表します。</span><span class="sxs-lookup"><span data-stu-id="7c416-122">Represents a distinguished folder name of the folder that contains the user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c416-123">親要素</span><span class="sxs-lookup"><span data-stu-id="7c416-123">Parent elements</span></span>

|<span data-ttu-id="7c416-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="7c416-124">**Element**</span></span>|<span data-ttu-id="7c416-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c416-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c416-126">DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c416-126">DeleteUserConfiguration</span></span>](deleteuserconfiguration.md) <br/> |<span data-ttu-id="7c416-127">ユーザーの構成オブジェクトを削除する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="7c416-127">Represents a request to delete a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="7c416-128">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c416-128">GetUserConfiguration</span></span>](getuserconfiguration.md) <br/> |<span data-ttu-id="7c416-129">ユーザーの構成オブジェクトを取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="7c416-129">Represents a request to get a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="7c416-130">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c416-130">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="7c416-131">1 人のユーザーの構成オブジェクトを定義します。</span><span class="sxs-lookup"><span data-stu-id="7c416-131">Defines a single user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7c416-132">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7c416-132">Text value</span></span>

<span data-ttu-id="7c416-133">なし。</span><span class="sxs-lookup"><span data-stu-id="7c416-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7c416-134">注釈</span><span class="sxs-lookup"><span data-stu-id="7c416-134">Remarks</span></span>

<span data-ttu-id="7c416-135">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7c416-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c416-136">要素情報</span><span class="sxs-lookup"><span data-stu-id="7c416-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c416-137">名前空間</span><span class="sxs-lookup"><span data-stu-id="7c416-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c416-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7c416-138">Schema Name</span></span>  <br/> |<span data-ttu-id="7c416-139">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7c416-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c416-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7c416-140">Validation File</span></span>  <br/> |<span data-ttu-id="7c416-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7c416-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c416-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7c416-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c416-143">False</span><span class="sxs-lookup"><span data-stu-id="7c416-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c416-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="7c416-144">See also</span></span>

- [<span data-ttu-id="7c416-145">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7c416-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

