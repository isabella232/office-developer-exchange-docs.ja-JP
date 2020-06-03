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
description: UserConfigurationName 要素は、ユーザー構成オブジェクトの名前を表します。 ユーザー構成オブジェクトの名前は、ユーザー構成オブジェクトの識別子です。
ms.openlocfilehash: 020b55919f7f81602a5eb072652d82168607d306
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466032"
---
# <a name="userconfigurationname"></a><span data-ttu-id="177d3-104">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="177d3-104">UserConfigurationName</span></span>

<span data-ttu-id="177d3-105">**Userconfigurationname**要素は、ユーザー構成オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="177d3-105">The **UserConfigurationName** element represents the name of a user configuration object.</span></span> <span data-ttu-id="177d3-106">ユーザー構成オブジェクトの名前は、ユーザー構成オブジェクトの識別子です。</span><span class="sxs-lookup"><span data-stu-id="177d3-106">The user configuration object name is the identifier for a user configuration object.</span></span> 
  
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

<span data-ttu-id="177d3-107">**UserConfigurationNameType**</span><span class="sxs-lookup"><span data-stu-id="177d3-107">**UserConfigurationNameType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="177d3-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="177d3-108">Attributes and elements</span></span>

<span data-ttu-id="177d3-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="177d3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="177d3-110">属性</span><span class="sxs-lookup"><span data-stu-id="177d3-110">Attributes</span></span>

|<span data-ttu-id="177d3-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="177d3-111">**Attribute**</span></span>|<span data-ttu-id="177d3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="177d3-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="177d3-113">**名前**</span><span class="sxs-lookup"><span data-stu-id="177d3-113">**Name**</span></span> <br/> |<span data-ttu-id="177d3-114">ユーザー構成オブジェクトの名前を表す文字列型 (string) の値を格納します。</span><span class="sxs-lookup"><span data-stu-id="177d3-114">Contains a string value that represents the name of a user configuration object.</span></span> <span data-ttu-id="177d3-115">この属性は必須です。</span><span class="sxs-lookup"><span data-stu-id="177d3-115">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="177d3-116">子要素</span><span class="sxs-lookup"><span data-stu-id="177d3-116">Child elements</span></span>

|<span data-ttu-id="177d3-117">**Element**</span><span class="sxs-lookup"><span data-stu-id="177d3-117">**Element**</span></span>|<span data-ttu-id="177d3-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="177d3-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="177d3-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="177d3-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="177d3-120">ユーザー構成オブジェクトを含むフォルダーのフォルダー識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="177d3-120">Represents the folder identifier of the folder that contains the user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="177d3-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="177d3-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="177d3-122">ユーザー構成オブジェクトを含むフォルダーの識別フォルダー名を表します。</span><span class="sxs-lookup"><span data-stu-id="177d3-122">Represents a distinguished folder name of the folder that contains the user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="177d3-123">親要素</span><span class="sxs-lookup"><span data-stu-id="177d3-123">Parent elements</span></span>

|<span data-ttu-id="177d3-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="177d3-124">**Element**</span></span>|<span data-ttu-id="177d3-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="177d3-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="177d3-126">DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="177d3-126">DeleteUserConfiguration</span></span>](deleteuserconfiguration.md) <br/> |<span data-ttu-id="177d3-127">ユーザー構成オブジェクトを削除する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="177d3-127">Represents a request to delete a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="177d3-128">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="177d3-128">GetUserConfiguration</span></span>](getuserconfiguration.md) <br/> |<span data-ttu-id="177d3-129">ユーザー構成オブジェクトを取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="177d3-129">Represents a request to get a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="177d3-130">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="177d3-130">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="177d3-131">1つのユーザー構成オブジェクトを定義します。</span><span class="sxs-lookup"><span data-stu-id="177d3-131">Defines a single user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="177d3-132">テキスト値</span><span class="sxs-lookup"><span data-stu-id="177d3-132">Text value</span></span>

<span data-ttu-id="177d3-133">なし。</span><span class="sxs-lookup"><span data-stu-id="177d3-133">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="177d3-134">注釈</span><span class="sxs-lookup"><span data-stu-id="177d3-134">Remarks</span></span>

<span data-ttu-id="177d3-135">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="177d3-135">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="177d3-136">要素の情報</span><span class="sxs-lookup"><span data-stu-id="177d3-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="177d3-137">Namespace</span><span class="sxs-lookup"><span data-stu-id="177d3-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="177d3-138">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="177d3-138">Schema Name</span></span>  <br/> |<span data-ttu-id="177d3-139">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="177d3-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="177d3-140">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="177d3-140">Validation File</span></span>  <br/> |<span data-ttu-id="177d3-141">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="177d3-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="177d3-142">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="177d3-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="177d3-143">正しくない</span><span class="sxs-lookup"><span data-stu-id="177d3-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="177d3-144">関連項目</span><span class="sxs-lookup"><span data-stu-id="177d3-144">See also</span></span>

- [<span data-ttu-id="177d3-145">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="177d3-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

