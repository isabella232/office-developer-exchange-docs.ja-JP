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
ms.openlocfilehash: 9003560a89b83032b4dd1b7ff54f3101819cc3c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832266"
---
# <a name="mailboxculture"></a><span data-ttu-id="56f72-104">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="56f72-104">MailboxCulture</span></span>

<span data-ttu-id="56f72-105">**MailboxCulture**要素は、メールボックスを開くときに使用するカルチャを示します。</span><span class="sxs-lookup"><span data-stu-id="56f72-105">The **MailboxCulture** element indicates the culture to use when opening a mailbox.</span></span> <span data-ttu-id="56f72-106">この要素は、SOAP ヘッダーで発生します。</span><span class="sxs-lookup"><span data-stu-id="56f72-106">This element occurs in the SOAP header.</span></span> 
  
```xml
<MailboxCulture/>
```

<span data-ttu-id="56f72-107">**MailboxCultureType**</span><span class="sxs-lookup"><span data-stu-id="56f72-107">**MailboxCultureType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="56f72-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="56f72-108">Attributes and elements</span></span>

<span data-ttu-id="56f72-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="56f72-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56f72-110">属性</span><span class="sxs-lookup"><span data-stu-id="56f72-110">Attributes</span></span>

<span data-ttu-id="56f72-111">なし。</span><span class="sxs-lookup"><span data-stu-id="56f72-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="56f72-112">子要素</span><span class="sxs-lookup"><span data-stu-id="56f72-112">Child elements</span></span>

<span data-ttu-id="56f72-113">なし。</span><span class="sxs-lookup"><span data-stu-id="56f72-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="56f72-114">親要素</span><span class="sxs-lookup"><span data-stu-id="56f72-114">Parent elements</span></span>

<span data-ttu-id="56f72-115">なし。</span><span class="sxs-lookup"><span data-stu-id="56f72-115">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="56f72-116">テキスト値</span><span class="sxs-lookup"><span data-stu-id="56f72-116">Text value</span></span>

<span data-ttu-id="56f72-117">テキスト値は、Exchange Web サービス操作で使用される言語を示します。</span><span class="sxs-lookup"><span data-stu-id="56f72-117">The text value indicates the language that is used in the Exchange Web Service operations.</span></span> <span data-ttu-id="56f72-118">RFC 3066 では、この要素の値が記載されています。</span><span class="sxs-lookup"><span data-stu-id="56f72-118">The possible values for this element are described by RFC 3066.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="56f72-119">備考</span><span class="sxs-lookup"><span data-stu-id="56f72-119">Remarks</span></span>

<span data-ttu-id="56f72-120">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="56f72-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56f72-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="56f72-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56f72-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="56f72-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="56f72-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="56f72-123">Schema Name</span></span>  <br/> |<span data-ttu-id="56f72-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="56f72-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="56f72-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="56f72-125">Validation File</span></span>  <br/> |<span data-ttu-id="56f72-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="56f72-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="56f72-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="56f72-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="56f72-128">False</span><span class="sxs-lookup"><span data-stu-id="56f72-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56f72-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="56f72-129">See also</span></span>

- [<span data-ttu-id="56f72-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="56f72-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

