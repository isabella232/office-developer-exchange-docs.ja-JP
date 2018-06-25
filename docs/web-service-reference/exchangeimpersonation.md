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
description: ExchangeImpersonation 要素は、要求の SOAP ヘッダーで使用されます。 この要素が存在する場合、呼び出し元が ExchangeImpersonation 要素内に含まれているアカウントを偽装するとしています。
ms.openlocfilehash: aedeff22cda865ce1eec80dab9760d49fdc178f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760357"
---
# <a name="exchangeimpersonation"></a><span data-ttu-id="042e5-104">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="042e5-104">ExchangeImpersonation</span></span>

<span data-ttu-id="042e5-105">**ExchangeImpersonation**要素は、要求の SOAP ヘッダーで使用されます。</span><span class="sxs-lookup"><span data-stu-id="042e5-105">The **ExchangeImpersonation** element is used in the SOAP header of a request.</span></span> <span data-ttu-id="042e5-106">この要素が存在する場合、呼び出し元が**ExchangeImpersonation**要素内に含まれているアカウントを偽装するとしています。</span><span class="sxs-lookup"><span data-stu-id="042e5-106">When this element is present, the caller is trying to impersonate the account that is contained within the **ExchangeImpersonation** element.</span></span> 
  
[<span data-ttu-id="042e5-107">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="042e5-107">ExchangeImpersonation</span></span>](exchangeimpersonation.md)
  
```xml
<ExchangeImpersonation>
   <ConnectingSID/>
</ExchangeImpersonation>
```

 <span data-ttu-id="042e5-108">**ExchangeImpersonationType**</span><span class="sxs-lookup"><span data-stu-id="042e5-108">**ExchangeImpersonationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="042e5-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="042e5-109">Attributes and elements</span></span>

<span data-ttu-id="042e5-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="042e5-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="042e5-111">属性</span><span class="sxs-lookup"><span data-stu-id="042e5-111">Attributes</span></span>

<span data-ttu-id="042e5-112">なし。</span><span class="sxs-lookup"><span data-stu-id="042e5-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="042e5-113">子要素</span><span class="sxs-lookup"><span data-stu-id="042e5-113">Child elements</span></span>

|<span data-ttu-id="042e5-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="042e5-114">**Element**</span></span>|<span data-ttu-id="042e5-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="042e5-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="042e5-116">ConnectingSID</span><span class="sxs-lookup"><span data-stu-id="042e5-116">ConnectingSID</span></span>](connectingsid.md) <br/> |<span data-ttu-id="042e5-117">ExchangeImpersonation SOAP ヘッダーを使用する際に偽装するアカウントを表します。</span><span class="sxs-lookup"><span data-stu-id="042e5-117">Represents an account to impersonate when you are using the ExchangeImpersonation SOAP header.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="042e5-118">親要素</span><span class="sxs-lookup"><span data-stu-id="042e5-118">Parent elements</span></span>

<span data-ttu-id="042e5-119">なし。</span><span class="sxs-lookup"><span data-stu-id="042e5-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="042e5-120">備考</span><span class="sxs-lookup"><span data-stu-id="042e5-120">Remarks</span></span>

<span data-ttu-id="042e5-121">呼び出し元のアカウントが必要でクライアント アクセス サーバーと**ms-exch-MayImpersonate** **ms の偽装 exch**上か、偽装するメールボックスを含むメールボックス データベースまたは Active Directory ユーザーと連絡先オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="042e5-121">The calling account must have the **ms-exch-impersonation** right on the Client Access server and the **ms-exch-MayImpersonate** right on either the mailbox database that contains the mailbox to impersonate or the Active Directory User/Contact object.</span></span> 
  
<span data-ttu-id="042e5-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="042e5-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="042e5-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="042e5-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="042e5-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="042e5-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="042e5-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="042e5-125">Schema name</span></span>  <br/> |<span data-ttu-id="042e5-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="042e5-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="042e5-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="042e5-127">Validation file</span></span>  <br/> |<span data-ttu-id="042e5-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="042e5-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="042e5-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="042e5-129">Can be empty</span></span>  <br/> |<span data-ttu-id="042e5-130">False</span><span class="sxs-lookup"><span data-stu-id="042e5-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="042e5-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="042e5-131">See also</span></span>



[<span data-ttu-id="042e5-132">EWS でのサーバーからサーバーへの承認</span><span class="sxs-lookup"><span data-stu-id="042e5-132">Server-to-server authorization in EWS</span></span>](http://msdn.microsoft.com/library/f1610a20-672d-448b-8c00-5b0fbcaf31cb%28Office.15%29.aspx)

