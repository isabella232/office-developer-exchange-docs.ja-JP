---
title: MailboxDataArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxDataArray
api_type:
- schema
ms.assetid: a14af788-beee-452c-b5d0-37bcb4ef02ff
description: MailboxDataArray 要素には、可用性情報を照会するメールボックスのリストが含まれています。
ms.openlocfilehash: 894bf97a0d633d7eef0434331ccf1580fcba386e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468195"
---
# <a name="mailboxdataarray"></a><span data-ttu-id="412ee-103">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="412ee-103">MailboxDataArray</span></span>

<span data-ttu-id="412ee-104">**MailboxDataArray**要素には、可用性情報を照会するメールボックスのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="412ee-104">The **MailboxDataArray** element contains a list of mailboxes to query for availability information.</span></span> 
  
- [<span data-ttu-id="412ee-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="412ee-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="412ee-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="412ee-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="412ee-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="412ee-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxDataArray>
   <MailboxData>...</MailboxData>
</MailboxDataArray>
```

<span data-ttu-id="412ee-108">**ArrayOfMailboxData**</span><span class="sxs-lookup"><span data-stu-id="412ee-108">**ArrayOfMailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="412ee-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="412ee-109">Attributes and elements</span></span>

<span data-ttu-id="412ee-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="412ee-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="412ee-111">属性</span><span class="sxs-lookup"><span data-stu-id="412ee-111">Attributes</span></span>

<span data-ttu-id="412ee-112">なし。</span><span class="sxs-lookup"><span data-stu-id="412ee-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="412ee-113">子要素</span><span class="sxs-lookup"><span data-stu-id="412ee-113">Child elements</span></span>

|<span data-ttu-id="412ee-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="412ee-114">**Element**</span></span>|<span data-ttu-id="412ee-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="412ee-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="412ee-116">MailboxData</span><span class="sxs-lookup"><span data-stu-id="412ee-116">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="412ee-117">個々のメールボックスユーザー、およびメールボックスユーザーに関して返されるデータの種類のオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="412ee-117">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="412ee-118">親要素</span><span class="sxs-lookup"><span data-stu-id="412ee-118">Parent elements</span></span>

|<span data-ttu-id="412ee-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="412ee-119">**Element**</span></span>|<span data-ttu-id="412ee-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="412ee-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="412ee-121">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="412ee-121">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="412ee-122">ユーザーの空き時間情報を取得するために使用する引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="412ee-122">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="412ee-123">これはルート要素です。</span><span class="sxs-lookup"><span data-stu-id="412ee-123">This is a root element.</span></span>  <br/> <span data-ttu-id="412ee-124">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="412ee-124">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="412ee-125">注釈</span><span class="sxs-lookup"><span data-stu-id="412ee-125">Remarks</span></span>

<span data-ttu-id="412ee-126">この要素を記述するスキーマは、Microsoft® Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="412ee-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="412ee-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="412ee-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="412ee-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="412ee-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="412ee-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="412ee-129">Schema Name</span></span>  <br/> |<span data-ttu-id="412ee-130">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="412ee-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="412ee-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="412ee-131">Validation File</span></span>  <br/> |<span data-ttu-id="412ee-132">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="412ee-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="412ee-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="412ee-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="412ee-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="412ee-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="412ee-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="412ee-135">See also</span></span>

- [<span data-ttu-id="412ee-136">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="412ee-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="412ee-137">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="412ee-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="412ee-138">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="412ee-138">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

