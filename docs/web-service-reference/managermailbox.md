---
title: ManagerMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 70c324d5-2196-406d-a674-73323f8d8b92
description: ManagerMailbox 要素には、連絡先のマネージャーのメールボックスを識別するための SMTP 情報が含まれています。
ms.openlocfilehash: b83ba2599cd56c9a1fd36132ac8eba0725616039
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832344"
---
# <a name="managermailbox"></a><span data-ttu-id="1268d-103">ManagerMailbox</span><span class="sxs-lookup"><span data-stu-id="1268d-103">ManagerMailbox</span></span>

<span data-ttu-id="1268d-104">**ManagerMailbox**要素には、連絡先のマネージャーのメールボックスを識別するための SMTP 情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1268d-104">The **ManagerMailbox** element contains SMTP information that identifies the mailbox of the contact's manager.</span></span> 
  
```XML
<ManagerMailbox/>
```

 <span data-ttu-id="1268d-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="1268d-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1268d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1268d-106">Attributes and elements</span></span>

<span data-ttu-id="1268d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1268d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1268d-108">属性</span><span class="sxs-lookup"><span data-stu-id="1268d-108">Attributes</span></span>

<span data-ttu-id="1268d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1268d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1268d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1268d-110">Child elements</span></span>

<span data-ttu-id="1268d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1268d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1268d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1268d-112">Parent elements</span></span>

|<span data-ttu-id="1268d-113">**要素名**</span><span class="sxs-lookup"><span data-stu-id="1268d-113">**Element name**</span></span>|<span data-ttu-id="1268d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1268d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1268d-115">Contact</span><span class="sxs-lookup"><span data-stu-id="1268d-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="1268d-116">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="1268d-116">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1268d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1268d-117">Text value</span></span>

<span data-ttu-id="1268d-118">なし。</span><span class="sxs-lookup"><span data-stu-id="1268d-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1268d-119">備考</span><span class="sxs-lookup"><span data-stu-id="1268d-119">Remarks</span></span>

<span data-ttu-id="1268d-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1268d-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="1268d-121">この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1268d-121">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1268d-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="1268d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1268d-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="1268d-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1268d-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1268d-124">Schema name</span></span>  <br/> |<span data-ttu-id="1268d-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="1268d-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="1268d-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1268d-126">Validation file</span></span>  <br/> |<span data-ttu-id="1268d-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1268d-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1268d-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1268d-128">Can be empty</span></span>  <br/> |<span data-ttu-id="1268d-129">False</span><span class="sxs-lookup"><span data-stu-id="1268d-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1268d-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="1268d-130">See also</span></span>



- [<span data-ttu-id="1268d-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1268d-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="1268d-132">連絡先 (Exchange Web サービス) を作成します。</span><span class="sxs-lookup"><span data-stu-id="1268d-132">Creating Contacts (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

