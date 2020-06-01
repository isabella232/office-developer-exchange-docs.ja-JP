---
title: ManagerMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 70c324d5-2196-406d-a674-73323f8d8b92
description: ManagerMailbox 要素には、連絡先の上司のメールボックスを識別する SMTP 情報が含まれています。
ms.openlocfilehash: da9e26c3efdd22000694839f5962a6bb0256f748
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44453967"
---
# <a name="managermailbox"></a><span data-ttu-id="042da-103">ManagerMailbox</span><span class="sxs-lookup"><span data-stu-id="042da-103">ManagerMailbox</span></span>

<span data-ttu-id="042da-104">**Managermailbox**要素には、連絡先の上司のメールボックスを識別する SMTP 情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="042da-104">The **ManagerMailbox** element contains SMTP information that identifies the mailbox of the contact's manager.</span></span> 
  
```XML
<ManagerMailbox/>
```

 <span data-ttu-id="042da-105">**SingleRecipientType**</span><span class="sxs-lookup"><span data-stu-id="042da-105">**SingleRecipientType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="042da-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="042da-106">Attributes and elements</span></span>

<span data-ttu-id="042da-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="042da-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="042da-108">属性</span><span class="sxs-lookup"><span data-stu-id="042da-108">Attributes</span></span>

<span data-ttu-id="042da-109">なし。</span><span class="sxs-lookup"><span data-stu-id="042da-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="042da-110">子要素</span><span class="sxs-lookup"><span data-stu-id="042da-110">Child elements</span></span>

<span data-ttu-id="042da-111">なし。</span><span class="sxs-lookup"><span data-stu-id="042da-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="042da-112">親要素</span><span class="sxs-lookup"><span data-stu-id="042da-112">Parent elements</span></span>

|<span data-ttu-id="042da-113">**要素名**</span><span class="sxs-lookup"><span data-stu-id="042da-113">**Element name**</span></span>|<span data-ttu-id="042da-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="042da-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="042da-115">連絡先</span><span class="sxs-lookup"><span data-stu-id="042da-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="042da-116">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="042da-116">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="042da-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="042da-117">Text value</span></span>

<span data-ttu-id="042da-118">なし。</span><span class="sxs-lookup"><span data-stu-id="042da-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="042da-119">注釈</span><span class="sxs-lookup"><span data-stu-id="042da-119">Remarks</span></span>

<span data-ttu-id="042da-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="042da-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="042da-121">この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="042da-121">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="042da-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="042da-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="042da-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="042da-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="042da-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="042da-124">Schema name</span></span>  <br/> |<span data-ttu-id="042da-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="042da-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="042da-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="042da-126">Validation file</span></span>  <br/> |<span data-ttu-id="042da-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="042da-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="042da-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="042da-128">Can be empty</span></span>  <br/> |<span data-ttu-id="042da-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="042da-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="042da-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="042da-130">See also</span></span>



- [<span data-ttu-id="042da-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="042da-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="042da-132">連絡先の作成 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="042da-132">Creating Contacts (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

