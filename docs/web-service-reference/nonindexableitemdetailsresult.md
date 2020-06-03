---
title: Nonindexableitemの取得結果
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7cbdbc21-5405-4cbc-8ca0-d7b0257927aa
description: Nonindexableitem詳細 Result 要素は、GetNonIndexableItemDetails WSDL 操作の結果を指定します。
ms.openlocfilehash: 647f58b5e7285af70bbfb3a203ba71c9a3ccebcc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465444"
---
# <a name="nonindexableitemdetailsresult"></a><span data-ttu-id="6c977-103">Nonindexableitemの取得結果</span><span class="sxs-lookup"><span data-stu-id="6c977-103">NonIndexableItemDetailsResult</span></span>

<span data-ttu-id="6c977-104">**Nonindexableitem詳細 result**要素は、 **getnonindexableitemdetails** WSDL 操作の結果を指定します。</span><span class="sxs-lookup"><span data-stu-id="6c977-104">The **NonIndexableItemDetailsResult** element specifies the results of the **GetNonIndexableItemDetails** WSDL operation.</span></span> 
  
```XML
<NonIndexableItemDetailsResult>
   <Items/>
   <FailedMailboxes/>
</NonIndexableItemDetailsResult>
```

 <span data-ttu-id="6c977-105">**Nonindexableitemの Resulttype**</span><span class="sxs-lookup"><span data-stu-id="6c977-105">**NonIndexableItemDetailResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6c977-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6c977-106">Attributes and elements</span></span>

<span data-ttu-id="6c977-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6c977-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c977-108">属性</span><span class="sxs-lookup"><span data-stu-id="6c977-108">Attributes</span></span>

<span data-ttu-id="6c977-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6c977-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c977-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6c977-110">Child elements</span></span>

<span data-ttu-id="6c977-111">[アイテム (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md) 、[失敗したメールボックス](failedmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="6c977-111">[Items (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md) , [FailedMailboxes](failedmailboxes.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6c977-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6c977-112">Parent elements</span></span>

<span data-ttu-id="6c977-113">[GetnonindexableitemGetNonIndexableItemDetailsResponseMessage の応答](getnonindexableitemdetailsresponse.md)、 [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)</span><span class="sxs-lookup"><span data-stu-id="6c977-113">[GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md) , [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6c977-114">注釈</span><span class="sxs-lookup"><span data-stu-id="6c977-114">Remarks</span></span>

<span data-ttu-id="6c977-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6c977-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6c977-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6c977-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6c977-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6c977-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6c977-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="6c977-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6c977-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6c977-119">Schema name</span></span>  <br/> |<span data-ttu-id="6c977-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="6c977-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6c977-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6c977-121">Validation file</span></span>  <br/> |<span data-ttu-id="6c977-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6c977-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6c977-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6c977-123">Can be empty</span></span>  <br/> |<span data-ttu-id="6c977-124">正しくない</span><span class="sxs-lookup"><span data-stu-id="6c977-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6c977-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="6c977-125">See also</span></span>



[<span data-ttu-id="6c977-126">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="6c977-126">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)


- [<span data-ttu-id="6c977-127">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6c977-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

