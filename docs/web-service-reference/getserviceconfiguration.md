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
ms.openlocfilehash: e9357a9e3be22e129c4910c01231f9dbd22a2dbe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457873"
---
# <a name="getserviceconfiguration"></a><span data-ttu-id="3585f-103">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="3585f-103">GetServiceConfiguration</span></span>

<span data-ttu-id="3585f-104">**GetServiceConfiguration**要素は、GetServiceConfiguration 要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="3585f-104">The **GetServiceConfiguration** element defines a GetServiceConfiguration request.</span></span> 
  
```XML
<GetServiceConfiguration>
   <ActingAs/>
   <RequestedConfiguration/>
</GetServiceConfiguration>
```

 <span data-ttu-id="3585f-105">**GetServiceConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="3585f-105">**GetServiceConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3585f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3585f-106">Attributes and elements</span></span>

<span data-ttu-id="3585f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3585f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3585f-108">属性</span><span class="sxs-lookup"><span data-stu-id="3585f-108">Attributes</span></span>

<span data-ttu-id="3585f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3585f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3585f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3585f-110">Child elements</span></span>

|<span data-ttu-id="3585f-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="3585f-111">**Element**</span></span>|<span data-ttu-id="3585f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3585f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3585f-113">ActingAs</span><span class="sxs-lookup"><span data-stu-id="3585f-113">ActingAs</span></span>](actingas.md) <br/> |<span data-ttu-id="3585f-114">発信者が送信者として送信しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="3585f-114">Identifies who the caller is sending as.</span></span> <span data-ttu-id="3585f-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="3585f-115">This element is optional.</span></span> <span data-ttu-id="3585f-116">この要素が存在しない場合、認証されたユーザーは送信者と見なされます。</span><span class="sxs-lookup"><span data-stu-id="3585f-116">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="3585f-117">送信者ヒントを要求するには、 **Actingas**要素を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="3585f-117">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="3585f-118">**Actingas**要素が存在しない場合、ルーティングの種類が含まれていない場合、電子メールアドレスが含まれていない場合、電子メールアドレスが含まれていない場合、Active Directory ドメインサービス (AD ds) 内のユーザーに解決されない場合、または ad ds 内の複数のユーザーに解決される場合は、応答で ErrorInvalidArgument</span><span class="sxs-lookup"><span data-stu-id="3585f-118">An ErrorInvalidArgument error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span>  <br/> |
|[<span data-ttu-id="3585f-119">RequestedConfiguration</span><span class="sxs-lookup"><span data-stu-id="3585f-119">RequestedConfiguration</span></span>](requestedconfiguration.md) <br/> |<span data-ttu-id="3585f-120">要求されたサービス構成を含みます。</span><span class="sxs-lookup"><span data-stu-id="3585f-120">Contains the requested service configurations.</span></span> <span data-ttu-id="3585f-121">この要素は必須です。</span><span class="sxs-lookup"><span data-stu-id="3585f-121">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3585f-122">親要素</span><span class="sxs-lookup"><span data-stu-id="3585f-122">Parent elements</span></span>

<span data-ttu-id="3585f-123">なし。</span><span class="sxs-lookup"><span data-stu-id="3585f-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3585f-124">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3585f-124">Text value</span></span>

<span data-ttu-id="3585f-125">なし。</span><span class="sxs-lookup"><span data-stu-id="3585f-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3585f-126">注釈</span><span class="sxs-lookup"><span data-stu-id="3585f-126">Remarks</span></span>

<span data-ttu-id="3585f-127">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3585f-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3585f-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3585f-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3585f-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="3585f-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3585f-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3585f-130">Schema Name</span></span>  <br/> |<span data-ttu-id="3585f-131">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="3585f-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3585f-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3585f-132">Validation File</span></span>  <br/> |<span data-ttu-id="3585f-133">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3585f-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3585f-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3585f-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="3585f-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="3585f-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3585f-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="3585f-136">See also</span></span>



- [<span data-ttu-id="3585f-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3585f-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

