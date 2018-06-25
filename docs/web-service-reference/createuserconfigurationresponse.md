---
title: CreateUserConfigurationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateUserConfigurationResponse
api_type:
- schema
ms.assetid: 115d4a5d-0c90-45d5-a3a3-4e61d80df78a
description: CreateUserConfigurationResponse 要素は、1 つの CreateUserConfiguration 要求への応答を定義します。
ms.openlocfilehash: b2ccbe6468481522536b4f0c3d5a4183b9887add
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759868"
---
# <a name="createuserconfigurationresponse"></a><span data-ttu-id="23f07-103">CreateUserConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="23f07-103">CreateUserConfigurationResponse</span></span>

<span data-ttu-id="23f07-104">**CreateUserConfigurationResponse**要素は、1 つの**CreateUserConfiguration**要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="23f07-104">The **CreateUserConfigurationResponse** element defines a response to a single **CreateUserConfiguration** request.</span></span> 
  
```xml
<CreateUserConfigurationResponse>
   <ResponseMessages/>
</CreateUserConfigurationResponse>
```

 <span data-ttu-id="23f07-105">**CreateUserConfigurationResponseType**</span><span class="sxs-lookup"><span data-stu-id="23f07-105">**CreateUserConfigurationResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23f07-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="23f07-106">Attributes and elements</span></span>

<span data-ttu-id="23f07-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="23f07-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23f07-108">属性</span><span class="sxs-lookup"><span data-stu-id="23f07-108">Attributes</span></span>

<span data-ttu-id="23f07-109">なし。</span><span class="sxs-lookup"><span data-stu-id="23f07-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23f07-110">子要素</span><span class="sxs-lookup"><span data-stu-id="23f07-110">Child elements</span></span>

|<span data-ttu-id="23f07-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="23f07-111">**Element**</span></span>|<span data-ttu-id="23f07-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="23f07-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23f07-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="23f07-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="23f07-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="23f07-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="23f07-115">親要素</span><span class="sxs-lookup"><span data-stu-id="23f07-115">Parent elements</span></span>

<span data-ttu-id="23f07-116">なし。</span><span class="sxs-lookup"><span data-stu-id="23f07-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="23f07-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="23f07-117">Text value</span></span>

<span data-ttu-id="23f07-118">なし。</span><span class="sxs-lookup"><span data-stu-id="23f07-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="23f07-119">備考</span><span class="sxs-lookup"><span data-stu-id="23f07-119">Remarks</span></span>

<span data-ttu-id="23f07-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="23f07-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23f07-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="23f07-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23f07-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="23f07-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="23f07-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="23f07-123">Schema Name</span></span>  <br/> |<span data-ttu-id="23f07-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="23f07-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="23f07-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="23f07-125">Validation File</span></span>  <br/> |<span data-ttu-id="23f07-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="23f07-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="23f07-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="23f07-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="23f07-128">False</span><span class="sxs-lookup"><span data-stu-id="23f07-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="23f07-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="23f07-129">See also</span></span>



- [<span data-ttu-id="23f07-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="23f07-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

