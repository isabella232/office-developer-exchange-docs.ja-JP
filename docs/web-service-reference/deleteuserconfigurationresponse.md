---
title: DeleteUserConfigurationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteUserConfigurationResponse
api_type:
- schema
ms.assetid: 034199c1-cdc3-48b8-a2cc-69bbfcdc5ce4
description: DeleteUserConfigurationResponse 要素は、1つの DeleteUserConfiguration 要求に対する応答を定義します。
ms.openlocfilehash: 2cf1e6d30f97d6ed819a1dc8259971ffc8c16435
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460744"
---
# <a name="deleteuserconfigurationresponse"></a><span data-ttu-id="51aef-103">DeleteUserConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="51aef-103">DeleteUserConfigurationResponse</span></span>

<span data-ttu-id="51aef-104">**Deleteuserconfigurationresponse**要素は、1つの**deleteuserconfiguration**要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="51aef-104">The **DeleteUserConfigurationResponse** element defines a response to a single **DeleteUserConfiguration** request.</span></span> 
  
```xml
<DeleteUserConfigurationResponse>   <ResponseMessages/></DeleteUserConfigurationResponse>
```

 <span data-ttu-id="51aef-105">**DeleteUserConfigurationResponseType**</span><span class="sxs-lookup"><span data-stu-id="51aef-105">**DeleteUserConfigurationResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="51aef-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="51aef-106">Attributes and elements</span></span>

<span data-ttu-id="51aef-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="51aef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51aef-108">属性</span><span class="sxs-lookup"><span data-stu-id="51aef-108">Attributes</span></span>

<span data-ttu-id="51aef-109">なし。</span><span class="sxs-lookup"><span data-stu-id="51aef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="51aef-110">子要素</span><span class="sxs-lookup"><span data-stu-id="51aef-110">Child elements</span></span>

|<span data-ttu-id="51aef-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="51aef-111">**Element**</span></span>|<span data-ttu-id="51aef-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="51aef-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51aef-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="51aef-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="51aef-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="51aef-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="51aef-115">親要素</span><span class="sxs-lookup"><span data-stu-id="51aef-115">Parent elements</span></span>

<span data-ttu-id="51aef-116">なし。</span><span class="sxs-lookup"><span data-stu-id="51aef-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="51aef-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="51aef-117">Text value</span></span>

<span data-ttu-id="51aef-118">なし。</span><span class="sxs-lookup"><span data-stu-id="51aef-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="51aef-119">注釈</span><span class="sxs-lookup"><span data-stu-id="51aef-119">Remarks</span></span>

<span data-ttu-id="51aef-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="51aef-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="51aef-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="51aef-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51aef-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="51aef-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="51aef-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="51aef-123">Schema Name</span></span>  <br/> |<span data-ttu-id="51aef-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="51aef-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="51aef-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="51aef-125">Validation File</span></span>  <br/> |<span data-ttu-id="51aef-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="51aef-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="51aef-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="51aef-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="51aef-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="51aef-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="51aef-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="51aef-129">See also</span></span>

- [<span data-ttu-id="51aef-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="51aef-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

