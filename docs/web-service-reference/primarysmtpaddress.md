---
title: PrimarySmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PrimarySmtpAddress
api_type:
- schema
ms.assetid: eee79904-9412-4e61-b9b8-aff0ce25fade
description: PrimarySmtpAddress 要素は、サーバーからサーバーへの認証に使用するか、代理アクセス権をアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。
ms.openlocfilehash: d33bf22af4ddf6b2f6d8d8d434168264acfaea7c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/15/2018
ms.locfileid: "19832881"
---
# <a name="primarysmtpaddress"></a><span data-ttu-id="44601-103">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="44601-103">PrimarySmtpAddress</span></span>

<span data-ttu-id="44601-104">**PrimarySmtpAddress**要素は、サーバーからサーバーへの認証に使用するか、代理アクセス権をアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="44601-104">The **PrimarySmtpAddress** element represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for server-to-server authorization or delegate access.</span></span> 
  
```xml
<PrimarySmtpAddress/>
```

 <span data-ttu-id="44601-105">**PrimarySmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="44601-105">**PrimarySmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="44601-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="44601-106">Attributes and elements</span></span>

<span data-ttu-id="44601-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="44601-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="44601-108">属性</span><span class="sxs-lookup"><span data-stu-id="44601-108">Attributes</span></span>

<span data-ttu-id="44601-109">なし。</span><span class="sxs-lookup"><span data-stu-id="44601-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="44601-110">子要素</span><span class="sxs-lookup"><span data-stu-id="44601-110">Child elements</span></span>

<span data-ttu-id="44601-111">なし。</span><span class="sxs-lookup"><span data-stu-id="44601-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="44601-112">親要素</span><span class="sxs-lookup"><span data-stu-id="44601-112">Parent elements</span></span>

|<span data-ttu-id="44601-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="44601-113">**Element**</span></span>|<span data-ttu-id="44601-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="44601-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="44601-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="44601-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="44601-116">ExchangeImpersonation SOAP ヘッダーを使用する際に偽装するアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="44601-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="44601-117">この要素への XPath 式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="44601-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="44601-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="44601-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="44601-119">サーバー間認証でトークンのシリアル化を SOAP ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="44601-119">Used in the SOAP header for token serialization in server- to-server authentication.</span></span>  <br/> |
|[<span data-ttu-id="44601-120">ユーザー Id</span><span class="sxs-lookup"><span data-stu-id="44601-120">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="44601-121">代理ユーザー、またはフォルダーのアクセス許可を持つユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="44601-121">Identifies a delegate user or a user who has folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="44601-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="44601-122">Text value</span></span>

<span data-ttu-id="44601-123">SMTP アドレスを表す文字列値は、必要があります。</span><span class="sxs-lookup"><span data-stu-id="44601-123">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="44601-124">Remarks</span><span class="sxs-lookup"><span data-stu-id="44601-124">Remarks</span></span>

<span data-ttu-id="44601-125">Exchange Web サービスでは、メールボックスが、メールボックスのプライマリ SMTP アドレスによって識別することが必要です。</span><span class="sxs-lookup"><span data-stu-id="44601-125">Exchange Web Services requires that mailboxes be identified by the primary SMTP address of the mailbox.</span></span> <span data-ttu-id="44601-126">プロキシ アドレスまたは代替アドレスは使用できません。</span><span class="sxs-lookup"><span data-stu-id="44601-126">Proxy or alternative addresses are not accepted.</span></span>
  
<span data-ttu-id="44601-127">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="44601-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="44601-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="44601-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="44601-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="44601-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="44601-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="44601-130">Schema Name</span></span>  <br/> |<span data-ttu-id="44601-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="44601-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="44601-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="44601-132">Validation File</span></span>  <br/> |<span data-ttu-id="44601-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="44601-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="44601-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="44601-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="44601-135">False</span><span class="sxs-lookup"><span data-stu-id="44601-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="44601-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="44601-136">See also</span></span>



- [<span data-ttu-id="44601-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="44601-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="44601-138">EWS でのサーバーからサーバーへの承認</span><span class="sxs-lookup"><span data-stu-id="44601-138">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)
  
[<span data-ttu-id="44601-139">代理人アクセスを使用します。</span><span class="sxs-lookup"><span data-stu-id="44601-139">Working with Delegate Access</span></span>](http://msdn.microsoft.com/library/dfd6b4a3-8fd3-47ba-83c0-52465cb5f3f3%28Office.15%29.aspx)

