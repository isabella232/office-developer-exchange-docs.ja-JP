---
title: GetServiceConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: acbb29e4-d853-4302-8e32-7018775d54e4
description: GetServiceConfiguration 要素は、GetServiceConfiguration 要求を定義します。
ms.openlocfilehash: 7ff7124ff062f21a02fc69b86b7cc7367ba3fcb6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831666"
---
# <a name="getserviceconfiguration"></a><span data-ttu-id="1cea0-103">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="1cea0-103">GetServiceConfiguration</span></span>

<span data-ttu-id="1cea0-104">**GetServiceConfiguration**要素は、GetServiceConfiguration 要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="1cea0-104">The **GetServiceConfiguration** element defines a GetServiceConfiguration request.</span></span> 
  
```XML
<GetServiceConfiguration>
   <ActingAs/>
   <RequestedConfiguration/>
</GetServiceConfiguration>
```

 <span data-ttu-id="1cea0-105">**GetServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="1cea0-105">**GetServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1cea0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1cea0-106">Attributes and elements</span></span>

<span data-ttu-id="1cea0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1cea0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1cea0-108">属性</span><span class="sxs-lookup"><span data-stu-id="1cea0-108">Attributes</span></span>

<span data-ttu-id="1cea0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1cea0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1cea0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1cea0-110">Child elements</span></span>

|<span data-ttu-id="1cea0-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="1cea0-111">**Element**</span></span>|<span data-ttu-id="1cea0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1cea0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1cea0-113">ActingAs</span><span class="sxs-lookup"><span data-stu-id="1cea0-113">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="1cea0-114">として送信する呼び出し元を識別します。</span><span class="sxs-lookup"><span data-stu-id="1cea0-114">Identifies who the caller is sending as.</span></span> <span data-ttu-id="1cea0-115">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="1cea0-115">This element is optional.</span></span> <span data-ttu-id="1cea0-116">この要素が存在しない場合は、認証されたユーザーは、送信者と見なされます。</span><span class="sxs-lookup"><span data-stu-id="1cea0-116">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="1cea0-117">**ActingAs**要素は、送信者のヒントを要求するために含まれていなければなりません。</span><span class="sxs-lookup"><span data-stu-id="1cea0-117">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="1cea0-118">**ActingAs**要素が不足している、ルーティングの種類が含まれていない、電子メール アドレスが含まれていない、無効な電子メール アドレスが含まれています、Active Directory ドメイン内のユーザーに解決されない場合、ErrorInvalidArgument エラーが応答で返されるサービス (AD DS)、または、AD DS 内の複数のユーザーに解決します。</span><span class="sxs-lookup"><span data-stu-id="1cea0-118">An ErrorInvalidArgument error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span>  <br/> |
|[<span data-ttu-id="1cea0-119">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="1cea0-119">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="1cea0-120">要求されたサービスの構成が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1cea0-120">Contains the requested service configurations.</span></span> <span data-ttu-id="1cea0-121">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="1cea0-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1cea0-122">親要素</span><span class="sxs-lookup"><span data-stu-id="1cea0-122">Parent elements</span></span>

<span data-ttu-id="1cea0-123">なし。</span><span class="sxs-lookup"><span data-stu-id="1cea0-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="1cea0-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1cea0-124">Text value</span></span>

<span data-ttu-id="1cea0-125">なし。</span><span class="sxs-lookup"><span data-stu-id="1cea0-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1cea0-126">備考</span><span class="sxs-lookup"><span data-stu-id="1cea0-126">Remarks</span></span>

<span data-ttu-id="1cea0-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1cea0-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1cea0-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="1cea0-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1cea0-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="1cea0-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1cea0-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1cea0-130">Schema Name</span></span>  <br/> |<span data-ttu-id="1cea0-131">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1cea0-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1cea0-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1cea0-132">Validation File</span></span>  <br/> |<span data-ttu-id="1cea0-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1cea0-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1cea0-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1cea0-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="1cea0-135">False</span><span class="sxs-lookup"><span data-stu-id="1cea0-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1cea0-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="1cea0-136">See also</span></span>



- [<span data-ttu-id="1cea0-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1cea0-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

