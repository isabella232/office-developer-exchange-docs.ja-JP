---
title: NonIndexableItemDetailsResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7cbdbc21-5405-4cbc-8ca0-d7b0257927aa
description: NonIndexableItemDetailsResult 要素は、GetNonIndexableItemDetails の WSDL 操作の結果を指定します。
ms.openlocfilehash: 6e271f2cf0e37f26b945332c94167b6a42354115
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832535"
---
# <a name="nonindexableitemdetailsresult"></a><span data-ttu-id="eb225-103">NonIndexableItemDetailsResult</span><span class="sxs-lookup"><span data-stu-id="eb225-103">NonIndexableItemDetailsResult</span></span>

<span data-ttu-id="eb225-104">**NonIndexableItemDetailsResult**要素は、 **GetNonIndexableItemDetails**の WSDL 操作の結果を指定します。</span><span class="sxs-lookup"><span data-stu-id="eb225-104">The **NonIndexableItemDetailsResult** element specifies the results of the **GetNonIndexableItemDetails** WSDL operation.</span></span> 
  
```XML
<NonIndexableItemDetailsResult>
   <Items/>
   <FailedMailboxes/>
</NonIndexableItemDetailsResult>
```

 <span data-ttu-id="eb225-105">**NonIndexableItemDetailResultType**</span><span class="sxs-lookup"><span data-stu-id="eb225-105">**NonIndexableItemDetailResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb225-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="eb225-106">Attributes and elements</span></span>

<span data-ttu-id="eb225-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="eb225-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb225-108">属性</span><span class="sxs-lookup"><span data-stu-id="eb225-108">Attributes</span></span>

<span data-ttu-id="eb225-109">なし。</span><span class="sxs-lookup"><span data-stu-id="eb225-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eb225-110">子要素</span><span class="sxs-lookup"><span data-stu-id="eb225-110">Child elements</span></span>

<span data-ttu-id="eb225-111">[アイテム (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md) 、 [FailedMailboxes](failedmailboxes.md)</span><span class="sxs-lookup"><span data-stu-id="eb225-111">[Items (ArrayOfNonIndexableItemDetailsType)](items-arrayofnonindexableitemdetailstype.md) , [FailedMailboxes](failedmailboxes.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eb225-112">親要素</span><span class="sxs-lookup"><span data-stu-id="eb225-112">Parent elements</span></span>

<span data-ttu-id="eb225-113">[GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md) 、 [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)</span><span class="sxs-lookup"><span data-stu-id="eb225-113">[GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md) , [GetNonIndexableItemDetailsResponseMessage](getnonindexableitemdetailsresponsemessage.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="eb225-114">備考</span><span class="sxs-lookup"><span data-stu-id="eb225-114">Remarks</span></span>

<span data-ttu-id="eb225-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="eb225-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="eb225-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="eb225-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb225-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="eb225-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb225-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="eb225-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="eb225-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="eb225-119">Schema name</span></span>  <br/> |<span data-ttu-id="eb225-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="eb225-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="eb225-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="eb225-121">Validation file</span></span>  <br/> |<span data-ttu-id="eb225-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="eb225-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eb225-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="eb225-123">Can be empty</span></span>  <br/> |<span data-ttu-id="eb225-124">False</span><span class="sxs-lookup"><span data-stu-id="eb225-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb225-125">関連項目</span><span class="sxs-lookup"><span data-stu-id="eb225-125">See also</span></span>



[<span data-ttu-id="eb225-126">GetNonIndexableItemDetails 操作</span><span class="sxs-lookup"><span data-stu-id="eb225-126">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)


- [<span data-ttu-id="eb225-127">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="eb225-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

