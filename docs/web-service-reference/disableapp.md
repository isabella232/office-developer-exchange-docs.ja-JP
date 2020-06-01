---
title: DisableApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 42d2a888-fa62-4970-8306-9ddde4eeb1f0
description: DisableApp 要素は、アプリを無効にする要求を指定します。
ms.openlocfilehash: e99464677dc34e011e45548083fb830b819649fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457824"
---
# <a name="disableapp"></a><span data-ttu-id="9e7a4-103">DisableApp</span><span class="sxs-lookup"><span data-stu-id="9e7a4-103">DisableApp</span></span>

<span data-ttu-id="9e7a4-104">**Disableapp**要素は、アプリを無効にする要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e7a4-104">The **DisableApp** element specifies a request to disable an app.</span></span> 
  
```XML
<DisableApp>
    <ID></ID>
    <DisableReason></DisableReason>
</DisableApp>
```

 <span data-ttu-id="9e7a4-105">**DisableAppType**</span><span class="sxs-lookup"><span data-stu-id="9e7a4-105">**DisableAppType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e7a4-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9e7a4-106">Attributes and elements</span></span>

<span data-ttu-id="9e7a4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9e7a4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e7a4-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e7a4-108">Attributes</span></span>

<span data-ttu-id="9e7a4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9e7a4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e7a4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9e7a4-110">Child elements</span></span>

|<span data-ttu-id="9e7a4-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="9e7a4-111">**Element**</span></span>|<span data-ttu-id="9e7a4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9e7a4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e7a4-113">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="9e7a4-113">ID (String)</span></span>](id-string.md) <br/> |<span data-ttu-id="9e7a4-114">アイテムの id を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e7a4-114">Specifies the identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="9e7a4-115">DisableReason</span><span class="sxs-lookup"><span data-stu-id="9e7a4-115">DisableReason</span></span>](disablereason.md) <br/> |<span data-ttu-id="9e7a4-116">アプリを無効にする理由を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e7a4-116">Specifies the reason for disabling an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9e7a4-117">親要素</span><span class="sxs-lookup"><span data-stu-id="9e7a4-117">Parent elements</span></span>

<span data-ttu-id="9e7a4-118">なし。</span><span class="sxs-lookup"><span data-stu-id="9e7a4-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9e7a4-119">注釈</span><span class="sxs-lookup"><span data-stu-id="9e7a4-119">Remarks</span></span>

<span data-ttu-id="9e7a4-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9e7a4-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9e7a4-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9e7a4-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e7a4-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9e7a4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e7a4-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="9e7a4-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9e7a4-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9e7a4-124">Schema Name</span></span>  <br/> |<span data-ttu-id="9e7a4-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="9e7a4-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="9e7a4-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9e7a4-126">Validation File</span></span>  <br/> |<span data-ttu-id="9e7a4-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9e7a4-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9e7a4-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9e7a4-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9e7a4-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="9e7a4-129">See also</span></span>

- [<span data-ttu-id="9e7a4-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9e7a4-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

