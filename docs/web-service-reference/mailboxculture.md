---
title: MailboxCulture
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxCulture
api_type:
- schema
ms.assetid: 105cc061-3c35-455f-b102-8023e2055632
description: MailboxCulture 要素は、メールボックスを開くときに使用するカルチャを示します。 この要素は、SOAP ヘッダーで発生します。
ms.openlocfilehash: 5760bac3b4589cdba599c5200db7d77b73855ca4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467810"
---
# <a name="mailboxculture"></a><span data-ttu-id="93c42-104">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="93c42-104">MailboxCulture</span></span>

<span data-ttu-id="93c42-105">**MailboxCulture**要素は、メールボックスを開くときに使用するカルチャを示します。</span><span class="sxs-lookup"><span data-stu-id="93c42-105">The **MailboxCulture** element indicates the culture to use when opening a mailbox.</span></span> <span data-ttu-id="93c42-106">この要素は、SOAP ヘッダーで発生します。</span><span class="sxs-lookup"><span data-stu-id="93c42-106">This element occurs in the SOAP header.</span></span> 
  
```xml
<MailboxCulture/>
```

<span data-ttu-id="93c42-107">**MailboxCultureType**</span><span class="sxs-lookup"><span data-stu-id="93c42-107">**MailboxCultureType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="93c42-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="93c42-108">Attributes and elements</span></span>

<span data-ttu-id="93c42-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="93c42-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93c42-110">属性</span><span class="sxs-lookup"><span data-stu-id="93c42-110">Attributes</span></span>

<span data-ttu-id="93c42-111">なし。</span><span class="sxs-lookup"><span data-stu-id="93c42-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93c42-112">子要素</span><span class="sxs-lookup"><span data-stu-id="93c42-112">Child elements</span></span>

<span data-ttu-id="93c42-113">なし。</span><span class="sxs-lookup"><span data-stu-id="93c42-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="93c42-114">親要素</span><span class="sxs-lookup"><span data-stu-id="93c42-114">Parent elements</span></span>

<span data-ttu-id="93c42-115">なし。</span><span class="sxs-lookup"><span data-stu-id="93c42-115">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="93c42-116">テキスト値</span><span class="sxs-lookup"><span data-stu-id="93c42-116">Text value</span></span>

<span data-ttu-id="93c42-117">テキスト値は、Exchange Web サービス操作で使用されている言語を示します。</span><span class="sxs-lookup"><span data-stu-id="93c42-117">The text value indicates the language that is used in the Exchange Web Service operations.</span></span> <span data-ttu-id="93c42-118">この要素に指定できる値は、RFC 3066 で記述されています。</span><span class="sxs-lookup"><span data-stu-id="93c42-118">The possible values for this element are described by RFC 3066.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="93c42-119">注釈</span><span class="sxs-lookup"><span data-stu-id="93c42-119">Remarks</span></span>

<span data-ttu-id="93c42-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="93c42-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93c42-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="93c42-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93c42-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="93c42-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="93c42-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="93c42-123">Schema Name</span></span>  <br/> |<span data-ttu-id="93c42-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="93c42-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="93c42-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="93c42-125">Validation File</span></span>  <br/> |<span data-ttu-id="93c42-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="93c42-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="93c42-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="93c42-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="93c42-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="93c42-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93c42-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="93c42-129">See also</span></span>

- [<span data-ttu-id="93c42-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="93c42-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

