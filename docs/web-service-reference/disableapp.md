---
title: DisableApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 42d2a888-fa62-4970-8306-9ddde4eeb1f0
description: DisableApp 要素は、アプリケーションを無効にする要求を指定します。
ms.openlocfilehash: d6d895d98fb368a6912f9111a4b934ba9631268e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760054"
---
# <a name="disableapp"></a><span data-ttu-id="df679-103">DisableApp</span><span class="sxs-lookup"><span data-stu-id="df679-103">DisableApp</span></span>

<span data-ttu-id="df679-104">**DisableApp**要素は、アプリケーションを無効にする要求を指定します。</span><span class="sxs-lookup"><span data-stu-id="df679-104">The **DisableApp** element specifies a request to disable an app.</span></span> 
  
```XML
<DisableApp>
    <ID></ID>
    <DisableReason></DisableReason>
</DisableApp>
```

 <span data-ttu-id="df679-105">**DisableAppType**</span><span class="sxs-lookup"><span data-stu-id="df679-105">**DisableAppType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="df679-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="df679-106">Attributes and elements</span></span>

<span data-ttu-id="df679-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="df679-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="df679-108">属性</span><span class="sxs-lookup"><span data-stu-id="df679-108">Attributes</span></span>

<span data-ttu-id="df679-109">なし。</span><span class="sxs-lookup"><span data-stu-id="df679-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="df679-110">子要素</span><span class="sxs-lookup"><span data-stu-id="df679-110">Child elements</span></span>

|<span data-ttu-id="df679-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="df679-111">**Element**</span></span>|<span data-ttu-id="df679-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="df679-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="df679-113">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="df679-113">ID (String)</span></span>](id-string.md) <br/> |<span data-ttu-id="df679-114">アイテムの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="df679-114">Specifies the identifier of an item.</span></span>  <br/> |
|[<span data-ttu-id="df679-115">DisableReason</span><span class="sxs-lookup"><span data-stu-id="df679-115">DisableReason</span></span>](disablereason.md) <br/> |<span data-ttu-id="df679-116">アプリケーションを無効にする理由を指定します。</span><span class="sxs-lookup"><span data-stu-id="df679-116">Specifies the reason for disabling an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="df679-117">親要素</span><span class="sxs-lookup"><span data-stu-id="df679-117">Parent elements</span></span>

<span data-ttu-id="df679-118">なし。</span><span class="sxs-lookup"><span data-stu-id="df679-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="df679-119">備考</span><span class="sxs-lookup"><span data-stu-id="df679-119">Remarks</span></span>

<span data-ttu-id="df679-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="df679-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="df679-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="df679-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="df679-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="df679-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="df679-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="df679-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="df679-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="df679-124">Schema Name</span></span>  <br/> |<span data-ttu-id="df679-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="df679-125">Message schema</span></span>  <br/> |
|<span data-ttu-id="df679-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="df679-126">Validation File</span></span>  <br/> |<span data-ttu-id="df679-127">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="df679-127">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="df679-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="df679-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="df679-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="df679-129">See also</span></span>

- [<span data-ttu-id="df679-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="df679-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

