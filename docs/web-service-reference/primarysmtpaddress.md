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
description: PrimarySmtpAddress 要素は、サーバー間の認証または代理人アクセスに使用されるアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。
ms.openlocfilehash: eea995b3e546d7e94e65cf9b230b639a781c4928
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467964"
---
# <a name="primarysmtpaddress"></a><span data-ttu-id="a06cd-103">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="a06cd-103">PrimarySmtpAddress</span></span>

<span data-ttu-id="a06cd-104">**Primarysmtpaddress**要素は、サーバー間の認証または代理人アクセスに使用されるアカウントのプライマリ簡易メール転送プロトコル (SMTP) アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="a06cd-104">The **PrimarySmtpAddress** element represents the primary Simple Mail Transfer Protocol (SMTP) address of an account to be used for server-to-server authorization or delegate access.</span></span> 
  
```xml
<PrimarySmtpAddress/>
```

 <span data-ttu-id="a06cd-105">**PrimarySmtpAddressType**</span><span class="sxs-lookup"><span data-stu-id="a06cd-105">**PrimarySmtpAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a06cd-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a06cd-106">Attributes and elements</span></span>

<span data-ttu-id="a06cd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a06cd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a06cd-108">属性</span><span class="sxs-lookup"><span data-stu-id="a06cd-108">Attributes</span></span>

<span data-ttu-id="a06cd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a06cd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a06cd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a06cd-110">Child elements</span></span>

<span data-ttu-id="a06cd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a06cd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a06cd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a06cd-112">Parent elements</span></span>

|<span data-ttu-id="a06cd-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a06cd-113">**Element**</span></span>|<span data-ttu-id="a06cd-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a06cd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a06cd-115">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="a06cd-115">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="a06cd-116">ExchangeImpersonation SOAP ヘッダーを使用しているときに偽装するアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="a06cd-116">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> <span data-ttu-id="a06cd-117">この要素の XPath 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a06cd-117">The following is the XPath expression to this element:</span></span>  <br/>  `/ExchangeImpersonation/ConnectingSID` <br/> |
|[<span data-ttu-id="a06cd-118">SerializedSecurityContext</span><span class="sxs-lookup"><span data-stu-id="a06cd-118">SerializedSecurityContext</span></span>](serializedsecuritycontext.md) <br/> |<span data-ttu-id="a06cd-119">サーバー間認証のトークンシリアル化のために SOAP ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="a06cd-119">Used in the SOAP header for token serialization in server- to-server authentication.</span></span>  <br/> |
|[<span data-ttu-id="a06cd-120">UserId</span><span class="sxs-lookup"><span data-stu-id="a06cd-120">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="a06cd-121">代理ユーザーまたはフォルダーのアクセス許可を持つユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="a06cd-121">Identifies a delegate user or a user who has folder access permissions.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a06cd-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a06cd-122">Text value</span></span>

<span data-ttu-id="a06cd-123">SMTP アドレスを表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="a06cd-123">A text value that represents an SMTP address is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a06cd-124">注釈</span><span class="sxs-lookup"><span data-stu-id="a06cd-124">Remarks</span></span>

<span data-ttu-id="a06cd-125">Exchange Web サービスでは、メールボックスのプライマリ SMTP アドレスによってメールボックスが識別される必要があります。</span><span class="sxs-lookup"><span data-stu-id="a06cd-125">Exchange Web Services requires that mailboxes be identified by the primary SMTP address of the mailbox.</span></span> <span data-ttu-id="a06cd-126">プロキシまたは代替アドレスは受け付けられません。</span><span class="sxs-lookup"><span data-stu-id="a06cd-126">Proxy or alternative addresses are not accepted.</span></span>
  
<span data-ttu-id="a06cd-127">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="a06cd-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a06cd-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a06cd-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a06cd-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="a06cd-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a06cd-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a06cd-130">Schema Name</span></span>  <br/> |<span data-ttu-id="a06cd-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a06cd-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="a06cd-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a06cd-132">Validation File</span></span>  <br/> |<span data-ttu-id="a06cd-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a06cd-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a06cd-134">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a06cd-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="a06cd-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="a06cd-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a06cd-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="a06cd-136">See also</span></span>



- [<span data-ttu-id="a06cd-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a06cd-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="a06cd-138">EWS でのサーバー間認証</span><span class="sxs-lookup"><span data-stu-id="a06cd-138">Server-to-server authorization in EWS</span></span>](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)
  
[<span data-ttu-id="a06cd-139">代理人アクセスを使用する</span><span class="sxs-lookup"><span data-stu-id="a06cd-139">Working with Delegate Access</span></span>](https://msdn.microsoft.com/library/dfd6b4a3-8fd3-47ba-83c0-52465cb5f3f3%28Office.15%29.aspx)

