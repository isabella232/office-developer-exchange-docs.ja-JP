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
description: DeleteUserConfiguration 要素は、ユーザーの構成オブジェクトを削除する要求を表します。
ms.openlocfilehash: e357c32f95cddc866b77b6f1172ab260837b061b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759989"
---
# <a name="deleteuserconfiguration"></a><span data-ttu-id="9e152-103">DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e152-103">DeleteUserConfiguration</span></span>

<span data-ttu-id="9e152-104">**DeleteUserConfiguration**要素は、ユーザーの構成オブジェクトを削除する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="9e152-104">The **DeleteUserConfiguration** element represents a request to delete a user configuration object.</span></span> 
  
```xml
<DeleteUserConfiguration>
   <UserConfigurationName/>
</DeleteUserConfiguration>
```

 <span data-ttu-id="9e152-105">**DeleteUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="9e152-105">**DeleteUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e152-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9e152-106">Attributes and elements</span></span>

<span data-ttu-id="9e152-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9e152-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e152-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e152-108">Attributes</span></span>

<span data-ttu-id="9e152-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9e152-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e152-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9e152-110">Child elements</span></span>

|<span data-ttu-id="9e152-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="9e152-111">**Element**</span></span>|<span data-ttu-id="9e152-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9e152-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e152-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="9e152-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="9e152-114">削除するユーザーの構成オブジェクトの名前を表します。</span><span class="sxs-lookup"><span data-stu-id="9e152-114">Represents the name of the user configuration object to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9e152-115">親要素</span><span class="sxs-lookup"><span data-stu-id="9e152-115">Parent elements</span></span>

<span data-ttu-id="9e152-116">なし。</span><span class="sxs-lookup"><span data-stu-id="9e152-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9e152-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9e152-117">Text value</span></span>

<span data-ttu-id="9e152-118">なし。</span><span class="sxs-lookup"><span data-stu-id="9e152-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9e152-119">備考</span><span class="sxs-lookup"><span data-stu-id="9e152-119">Remarks</span></span>

<span data-ttu-id="9e152-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9e152-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e152-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="9e152-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e152-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="9e152-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9e152-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9e152-123">Schema Name</span></span>  <br/> |<span data-ttu-id="9e152-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9e152-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9e152-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9e152-125">Validation File</span></span>  <br/> |<span data-ttu-id="9e152-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9e152-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9e152-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9e152-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e152-128">False</span><span class="sxs-lookup"><span data-stu-id="9e152-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e152-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="9e152-129">See also</span></span>

- [<span data-ttu-id="9e152-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9e152-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

