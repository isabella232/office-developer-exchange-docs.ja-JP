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
description: CreateUserConfiguration 要素は、ユーザーの構成オブジェクトを作成する要求を表します。
ms.openlocfilehash: dcf3acc356110b993bdb7f4f83245753835f299f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759865"
---
# <a name="createuserconfiguration"></a><span data-ttu-id="2fd05-103">CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="2fd05-103">CreateUserConfiguration</span></span>

<span data-ttu-id="2fd05-104">**CreateUserConfiguration**要素は、ユーザーの構成オブジェクトを作成する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="2fd05-104">The **CreateUserConfiguration** element represents a request to create a user configuration object.</span></span> 
  
```xml
<CreateUserConfiguration>
   <UserConfiguration/>
</CreateUserConfiguration>
```

 <span data-ttu-id="2fd05-105">**CreateUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="2fd05-105">**CreateUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2fd05-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2fd05-106">Attributes and elements</span></span>

<span data-ttu-id="2fd05-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2fd05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2fd05-108">属性</span><span class="sxs-lookup"><span data-stu-id="2fd05-108">Attributes</span></span>

<span data-ttu-id="2fd05-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2fd05-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2fd05-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2fd05-110">Child elements</span></span>

|<span data-ttu-id="2fd05-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2fd05-111">**Element**</span></span>|<span data-ttu-id="2fd05-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2fd05-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2fd05-113">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="2fd05-113">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="2fd05-114">1 人のユーザーの構成オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="2fd05-114">Represents a single user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2fd05-115">親要素</span><span class="sxs-lookup"><span data-stu-id="2fd05-115">Parent elements</span></span>

<span data-ttu-id="2fd05-116">なし。</span><span class="sxs-lookup"><span data-stu-id="2fd05-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="2fd05-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2fd05-117">Text value</span></span>

<span data-ttu-id="2fd05-118">なし。</span><span class="sxs-lookup"><span data-stu-id="2fd05-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2fd05-119">備考</span><span class="sxs-lookup"><span data-stu-id="2fd05-119">Remarks</span></span>

<span data-ttu-id="2fd05-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2fd05-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2fd05-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="2fd05-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2fd05-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="2fd05-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2fd05-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2fd05-123">Schema Name</span></span>  <br/> |<span data-ttu-id="2fd05-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="2fd05-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2fd05-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2fd05-125">Validation File</span></span>  <br/> |<span data-ttu-id="2fd05-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2fd05-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2fd05-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2fd05-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="2fd05-128">False</span><span class="sxs-lookup"><span data-stu-id="2fd05-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2fd05-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="2fd05-129">See also</span></span>



- [<span data-ttu-id="2fd05-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2fd05-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

