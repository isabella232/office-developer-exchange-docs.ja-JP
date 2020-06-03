---
title: ExchangeImpersonation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExchangeImpersonation
api_type:
- schema
ms.assetid: d8cbac49-47d0-4745-a2a7-545d33f8da93
description: ExchangeImpersonation 要素は、要求の SOAP ヘッダーで使用されます。 この要素が存在する場合、発信者は ExchangeImpersonation 要素内に含まれるアカウントを偽装しようとしています。
ms.openlocfilehash: 188219d95453dc45378c6ca65ab93c2de7db4eac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463350"
---
# <a name="exchangeimpersonation"></a><span data-ttu-id="f94fa-104">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="f94fa-104">ExchangeImpersonation</span></span>

<span data-ttu-id="f94fa-105">**ExchangeImpersonation** 要素は、要求の SOAP ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="f94fa-105">The **ExchangeImpersonation** element is used in the SOAP header of a request.</span></span> <span data-ttu-id="f94fa-106">この要素が存在する場合、発信者は**Exchangeimpersonation**要素内に含まれるアカウントを偽装しようとしています。</span><span class="sxs-lookup"><span data-stu-id="f94fa-106">When this element is present, the caller is trying to impersonate the account that is contained within the **ExchangeImpersonation** element.</span></span> 
  
[<span data-ttu-id="f94fa-107">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="f94fa-107">ExchangeImpersonation</span></span>](exchangeimpersonation.md)
  
```xml
<ExchangeImpersonation>
   <ConnectingSID/>
</ExchangeImpersonation>
```

 <span data-ttu-id="f94fa-108">**ExchangeImpersonationType**</span><span class="sxs-lookup"><span data-stu-id="f94fa-108">**ExchangeImpersonationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f94fa-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f94fa-109">Attributes and elements</span></span>

<span data-ttu-id="f94fa-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f94fa-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f94fa-111">属性</span><span class="sxs-lookup"><span data-stu-id="f94fa-111">Attributes</span></span>

<span data-ttu-id="f94fa-112">なし。</span><span class="sxs-lookup"><span data-stu-id="f94fa-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f94fa-113">子要素</span><span class="sxs-lookup"><span data-stu-id="f94fa-113">Child elements</span></span>

|<span data-ttu-id="f94fa-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="f94fa-114">**Element**</span></span>|<span data-ttu-id="f94fa-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="f94fa-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f94fa-116">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="f94fa-116">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="f94fa-117">ExchangeImpersonation SOAP ヘッダーを使用しているときに偽装するアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="f94fa-117">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f94fa-118">親要素</span><span class="sxs-lookup"><span data-stu-id="f94fa-118">Parent elements</span></span>

<span data-ttu-id="f94fa-119">なし。</span><span class="sxs-lookup"><span data-stu-id="f94fa-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f94fa-120">注釈</span><span class="sxs-lookup"><span data-stu-id="f94fa-120">Remarks</span></span>

<span data-ttu-id="f94fa-121">呼び出し元のアカウントには、クライアントアクセスサーバーに**exch**権限が必要です。または、偽装するメールボックスを含むメールボックスデータベース、または Active Directory ユーザー/連絡先オブジェクトのいずれかに、 **exch**という権限が必要です。</span><span class="sxs-lookup"><span data-stu-id="f94fa-121">The calling account must have the **ms-exch-impersonation** right on the Client Access server and the **ms-exch-MayImpersonate** right on either the mailbox database that contains the mailbox to impersonate or the Active Directory User/Contact object.</span></span> 
  
<span data-ttu-id="f94fa-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f94fa-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f94fa-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f94fa-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f94fa-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="f94fa-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f94fa-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f94fa-125">Schema name</span></span>  <br/> |<span data-ttu-id="f94fa-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f94fa-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="f94fa-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f94fa-127">Validation file</span></span>  <br/> |<span data-ttu-id="f94fa-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f94fa-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f94fa-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f94fa-129">Can be empty</span></span>  <br/> |<span data-ttu-id="f94fa-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="f94fa-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f94fa-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="f94fa-131">See also</span></span>



[<span data-ttu-id="f94fa-132">EWS でのサーバー間認証</span><span class="sxs-lookup"><span data-stu-id="f94fa-132">Server-to-server authorization in EWS</span></span>](https://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

