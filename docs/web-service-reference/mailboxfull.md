---
title: MailboxFull
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxFull
api_type:
- schema
ms.assetid: 38b28c9b-9da2-4d6a-9cda-9c393986575b
description: MailboxFull 要素は、受信者のメールボックスがいっぱいになっているかどうかを示します。
ms.openlocfilehash: f336f1eda122bb170aafb22a028e3faf84f4d782
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465976"
---
# <a name="mailboxfull"></a><span data-ttu-id="ff756-103">MailboxFull</span><span class="sxs-lookup"><span data-stu-id="ff756-103">MailboxFull</span></span>

<span data-ttu-id="ff756-104">**MailboxFull**要素は、受信者のメールボックスがいっぱいになっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ff756-104">The **MailboxFull** element indicates whether the mailbox for the recipient is full.</span></span> 
  
```XML
<MailboxFull>true | false</MailboxFull>
```

<span data-ttu-id="ff756-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ff756-105">**Boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ff756-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ff756-106">Attributes and elements</span></span>

<span data-ttu-id="ff756-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ff756-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff756-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff756-108">Attributes</span></span>

<span data-ttu-id="ff756-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ff756-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff756-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ff756-110">Child elements</span></span>

<span data-ttu-id="ff756-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ff756-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ff756-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ff756-112">Parent elements</span></span>

|<span data-ttu-id="ff756-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ff756-113">**Element**</span></span>|<span data-ttu-id="ff756-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ff756-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff756-115">メールヒント</span><span class="sxs-lookup"><span data-stu-id="ff756-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="ff756-116">さまざまな種類のメールヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="ff756-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ff756-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ff756-117">Text value</span></span>

<span data-ttu-id="ff756-118">この要素は、 **true**または**false**のいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="ff756-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="ff756-119">値**true**は、メールボックスが容量に達したことを示します。値が**false**の場合は、容量に達していないことを示します。</span><span class="sxs-lookup"><span data-stu-id="ff756-119">A value of **true** indicates that the mailbox has reached its capacity; a value of **false** indicates that it has not reached capacity.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ff756-120">注釈</span><span class="sxs-lookup"><span data-stu-id="ff756-120">Remarks</span></span>

<span data-ttu-id="ff756-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ff756-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff756-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ff756-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff756-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="ff756-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ff756-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ff756-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ff756-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ff756-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="ff756-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ff756-126">Validation File</span></span>  <br/> |<span data-ttu-id="ff756-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ff756-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ff756-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ff756-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff756-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="ff756-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff756-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="ff756-130">See also</span></span>

- [<span data-ttu-id="ff756-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ff756-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

