---
title: ActingAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ActingAs
api_type:
- schema
ms.assetid: 3896afff-5c2c-4eaf-8621-c70e0371ea78
description: ActingAs 要素は、発信者が送信者を送信しているユーザーを識別します。
ms.openlocfilehash: 175a03018ee3529ec595dbe9afb7dc61ad6afc35
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529701"
---
# <a name="actingas"></a><span data-ttu-id="828f3-103">ActingAs</span><span class="sxs-lookup"><span data-stu-id="828f3-103">ActingAs</span></span>

<span data-ttu-id="828f3-104">**Actingas**要素は、発信者が送信者を送信しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="828f3-104">The **ActingAs** element identifies who the caller is sending as.</span></span> 
  
```xml
<ActingAs>
   <EmailAddress/>
   <RoutingType/>
</ActingAs>
```

 <span data-ttu-id="828f3-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="828f3-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="828f3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="828f3-106">Attributes and elements</span></span>

<span data-ttu-id="828f3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="828f3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="828f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="828f3-108">Attributes</span></span>

<span data-ttu-id="828f3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="828f3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="828f3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="828f3-110">Child elements</span></span>

|<span data-ttu-id="828f3-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="828f3-111">**Element**</span></span>|<span data-ttu-id="828f3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="828f3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="828f3-113">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="828f3-113">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="828f3-114">メールボックスユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="828f3-114">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="828f3-115">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="828f3-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="828f3-116">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="828f3-116">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="828f3-117">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="828f3-117">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="828f3-118">既定値は SMTP です。</span><span class="sxs-lookup"><span data-stu-id="828f3-118">The default is SMTP.</span></span> <span data-ttu-id="828f3-119">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="828f3-119">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="828f3-120">親要素</span><span class="sxs-lookup"><span data-stu-id="828f3-120">Parent elements</span></span>

|<span data-ttu-id="828f3-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="828f3-121">**Element**</span></span>|<span data-ttu-id="828f3-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="828f3-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="828f3-123">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="828f3-123">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="828f3-124">**GetServiceConfiguration**要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="828f3-124">Defines a **GetServiceConfiguration** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="828f3-125">注釈</span><span class="sxs-lookup"><span data-stu-id="828f3-125">Remarks</span></span>

<span data-ttu-id="828f3-126">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="828f3-126">This element is optional.</span></span> <span data-ttu-id="828f3-127">この要素が存在しない場合、認証されたユーザーは送信者と見なされます。</span><span class="sxs-lookup"><span data-stu-id="828f3-127">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="828f3-128">送信者ヒントを要求するには、 **Actingas**要素を含める必要があります。</span><span class="sxs-lookup"><span data-stu-id="828f3-128">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="828f3-129">**Actingas**要素が存在しない場合、ルーティングの種類が含まれていない場合、電子メールアドレスが含まれていない場合、電子メールアドレスが含まれていない場合、Active Directory ドメインサービス (AD ds) 内のユーザーに解決されない場合、または ad ds 内の複数のユーザーに解決される場合は、応答で**ErrorInvalidArgument**</span><span class="sxs-lookup"><span data-stu-id="828f3-129">An **ErrorInvalidArgument** error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span> 
  
<span data-ttu-id="828f3-130">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="828f3-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="828f3-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="828f3-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="828f3-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="828f3-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="828f3-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="828f3-133">Schema Name</span></span>  <br/> |<span data-ttu-id="828f3-134">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="828f3-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="828f3-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="828f3-135">Validation File</span></span>  <br/> |<span data-ttu-id="828f3-136">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="828f3-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="828f3-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="828f3-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="828f3-138">正しくない</span><span class="sxs-lookup"><span data-stu-id="828f3-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="828f3-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="828f3-139">See also</span></span>

- [<span data-ttu-id="828f3-140">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="828f3-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

