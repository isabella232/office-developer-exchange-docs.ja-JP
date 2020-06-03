---
title: DeleteUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteUserConfiguration
api_type:
- schema
ms.assetid: 91b18b6a-d904-476c-996d-b041e859da1e
description: DeleteUserConfiguration 要素は、ユーザー構成オブジェクトを削除するための要求を表します。
ms.openlocfilehash: 04668ead48e7c321ed7e91cbbeb67c6154c02283
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460758"
---
# <a name="deleteuserconfiguration"></a><span data-ttu-id="0c30a-103">DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="0c30a-103">DeleteUserConfiguration</span></span>

<span data-ttu-id="0c30a-104">**Deleteuserconfiguration**要素は、ユーザー構成オブジェクトを削除するための要求を表します。</span><span class="sxs-lookup"><span data-stu-id="0c30a-104">The **DeleteUserConfiguration** element represents a request to delete a user configuration object.</span></span> 
  
```xml
<DeleteUserConfiguration>
   <UserConfigurationName/>
</DeleteUserConfiguration>
```

 <span data-ttu-id="0c30a-105">**DeleteUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="0c30a-105">**DeleteUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0c30a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0c30a-106">Attributes and elements</span></span>

<span data-ttu-id="0c30a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0c30a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0c30a-108">属性</span><span class="sxs-lookup"><span data-stu-id="0c30a-108">Attributes</span></span>

<span data-ttu-id="0c30a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0c30a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0c30a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0c30a-110">Child elements</span></span>

|<span data-ttu-id="0c30a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="0c30a-111">**Element**</span></span>|<span data-ttu-id="0c30a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0c30a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c30a-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="0c30a-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="0c30a-114">削除するユーザー構成オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="0c30a-114">Represents the name of the user configuration object to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0c30a-115">親要素</span><span class="sxs-lookup"><span data-stu-id="0c30a-115">Parent elements</span></span>

<span data-ttu-id="0c30a-116">なし。</span><span class="sxs-lookup"><span data-stu-id="0c30a-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="0c30a-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0c30a-117">Text value</span></span>

<span data-ttu-id="0c30a-118">なし。</span><span class="sxs-lookup"><span data-stu-id="0c30a-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0c30a-119">注釈</span><span class="sxs-lookup"><span data-stu-id="0c30a-119">Remarks</span></span>

<span data-ttu-id="0c30a-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0c30a-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0c30a-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0c30a-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0c30a-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="0c30a-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0c30a-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0c30a-123">Schema Name</span></span>  <br/> |<span data-ttu-id="0c30a-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0c30a-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0c30a-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0c30a-125">Validation File</span></span>  <br/> |<span data-ttu-id="0c30a-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0c30a-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0c30a-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0c30a-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="0c30a-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="0c30a-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0c30a-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="0c30a-129">See also</span></span>

- [<span data-ttu-id="0c30a-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0c30a-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

