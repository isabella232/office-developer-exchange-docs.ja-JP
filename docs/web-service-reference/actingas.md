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
description: ActingAs 要素として、呼び出し元を送信するユーザーを識別します。
ms.openlocfilehash: 9c007ed45f85dba265261dd79a6fd846dbd9d2f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760452"
---
# <a name="actingas"></a><span data-ttu-id="9d47a-103">ActingAs</span><span class="sxs-lookup"><span data-stu-id="9d47a-103">ActingAs</span></span>

<span data-ttu-id="9d47a-104">**ActingAs**要素として、呼び出し元を送信するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="9d47a-104">The **ActingAs** element identifies who the caller is sending as.</span></span> 
  
```xml
<ActingAs>
   <EmailAddress/>
   <RoutingType/>
</ActingAs>
```

 <span data-ttu-id="9d47a-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="9d47a-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d47a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9d47a-106">Attributes and elements</span></span>

<span data-ttu-id="9d47a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9d47a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d47a-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d47a-108">Attributes</span></span>

<span data-ttu-id="9d47a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9d47a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d47a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9d47a-110">Child elements</span></span>

|<span data-ttu-id="9d47a-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="9d47a-111">**Element**</span></span>|<span data-ttu-id="9d47a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9d47a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d47a-113">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="9d47a-113">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="9d47a-114">メールボックスのユーザーの簡易メール転送プロトコル (SMTP) アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="9d47a-114">Defines the Simple Mail Transfer Protocol (SMTP) address of a mailbox user.</span></span> <span data-ttu-id="9d47a-115">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="9d47a-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9d47a-116">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="9d47a-116">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md) <br/> |<span data-ttu-id="9d47a-117">メールボックスに使用されるルーティングを定義します。</span><span class="sxs-lookup"><span data-stu-id="9d47a-117">Defines the routing that is used for the mailbox.</span></span> <span data-ttu-id="9d47a-118">既定値は、SMTP です。</span><span class="sxs-lookup"><span data-stu-id="9d47a-118">The default is SMTP.</span></span> <span data-ttu-id="9d47a-119">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="9d47a-119">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d47a-120">親要素</span><span class="sxs-lookup"><span data-stu-id="9d47a-120">Parent elements</span></span>

|<span data-ttu-id="9d47a-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="9d47a-121">**Element**</span></span>|<span data-ttu-id="9d47a-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="9d47a-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d47a-123">GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="9d47a-123">GetServiceConfiguration</span></span>](getserviceconfiguration.md) <br/> |<span data-ttu-id="9d47a-124">**GetServiceConfiguration**要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="9d47a-124">Defines a **GetServiceConfiguration** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9d47a-125">備考</span><span class="sxs-lookup"><span data-stu-id="9d47a-125">Remarks</span></span>

<span data-ttu-id="9d47a-126">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="9d47a-126">This element is optional.</span></span> <span data-ttu-id="9d47a-127">この要素が存在しない場合は、認証されたユーザーは、送信者と見なされます。</span><span class="sxs-lookup"><span data-stu-id="9d47a-127">If this element is not present, the authenticated user is assumed to be the sender.</span></span> <span data-ttu-id="9d47a-128">**ActingAs**要素は、送信者のヒントを要求するために含まれていなければなりません。</span><span class="sxs-lookup"><span data-stu-id="9d47a-128">The **ActingAs** element must be included for requesting sender hints.</span></span> <span data-ttu-id="9d47a-129">**ActingAs**要素が不足している、ルーティングの種類が含まれていない、電子メール アドレスが含まれていない、無効な電子メール アドレスが含まれています、Active Directory 内のユーザーに解決されない場合、 **ErrorInvalidArgument**エラーが応答で返されるドメイン サービス (AD DS)、または AD DS 内の複数のユーザーを解決します。</span><span class="sxs-lookup"><span data-stu-id="9d47a-129">An **ErrorInvalidArgument** error can be returned in a response if the **ActingAs** element is missing, does not include a routing type, does not include an e-mail address, contains an invalid e-mail address, does not resolve to a user in Active Directory Domain Services (AD DS), or resolves to multiple users in AD DS.</span></span> 
  
<span data-ttu-id="9d47a-130">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9d47a-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d47a-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="9d47a-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d47a-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="9d47a-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9d47a-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9d47a-133">Schema Name</span></span>  <br/> |<span data-ttu-id="9d47a-134">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9d47a-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9d47a-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9d47a-135">Validation File</span></span>  <br/> |<span data-ttu-id="9d47a-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9d47a-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9d47a-137">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9d47a-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d47a-138">False</span><span class="sxs-lookup"><span data-stu-id="9d47a-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d47a-139">関連項目</span><span class="sxs-lookup"><span data-stu-id="9d47a-139">See also</span></span>

- [<span data-ttu-id="9d47a-140">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9d47a-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

