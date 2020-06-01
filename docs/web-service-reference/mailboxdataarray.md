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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468195"
---
# <a name="mailboxdataarray"></a><span data-ttu-id="e9e14-103">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="e9e14-103">MailboxDataArray</span></span>

<span data-ttu-id="e9e14-104">**MailboxDataArray**要素には、可用性情報を照会するメールボックスのリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9e14-104">The **MailboxDataArray** element contains a list of mailboxes to query for availability information.</span></span> 
  
- [<span data-ttu-id="e9e14-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="e9e14-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="e9e14-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="e9e14-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="e9e14-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="e9e14-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxDataArray>
   <MailboxData>...</MailboxData>
</MailboxDataArray>
```

<span data-ttu-id="e9e14-108">**ArrayOfMailboxData**</span><span class="sxs-lookup"><span data-stu-id="e9e14-108">**ArrayOfMailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e9e14-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e9e14-109">Attributes and elements</span></span>

<span data-ttu-id="e9e14-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e9e14-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9e14-111">属性</span><span class="sxs-lookup"><span data-stu-id="e9e14-111">Attributes</span></span>

<span data-ttu-id="e9e14-112">なし。</span><span class="sxs-lookup"><span data-stu-id="e9e14-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9e14-113">子要素</span><span class="sxs-lookup"><span data-stu-id="e9e14-113">Child elements</span></span>

|<span data-ttu-id="e9e14-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="e9e14-114">**Element**</span></span>|<span data-ttu-id="e9e14-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9e14-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9e14-116">MailboxData</span><span class="sxs-lookup"><span data-stu-id="e9e14-116">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="e9e14-117">個々のメールボックスユーザー、およびメールボックスユーザーに関して返されるデータの種類のオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="e9e14-117">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9e14-118">親要素</span><span class="sxs-lookup"><span data-stu-id="e9e14-118">Parent elements</span></span>

|<span data-ttu-id="e9e14-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="e9e14-119">**Element**</span></span>|<span data-ttu-id="e9e14-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="e9e14-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9e14-121">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="e9e14-121">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="e9e14-122">ユーザーの空き時間情報を取得するために使用する引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9e14-122">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="e9e14-123">これはルート要素です。</span><span class="sxs-lookup"><span data-stu-id="e9e14-123">This is a root element.</span></span>  <br/> <span data-ttu-id="e9e14-124">この要素の XPath を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9e14-124">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e9e14-125">注釈</span><span class="sxs-lookup"><span data-stu-id="e9e14-125">Remarks</span></span>

<span data-ttu-id="e9e14-126">この要素を記述するスキーマは、Microsoft® Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="e9e14-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9e14-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e9e14-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9e14-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="e9e14-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e9e14-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e9e14-129">Schema Name</span></span>  <br/> |<span data-ttu-id="e9e14-130">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="e9e14-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e9e14-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e9e14-131">Validation File</span></span>  <br/> |<span data-ttu-id="e9e14-132">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="e9e14-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e9e14-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e9e14-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9e14-134">正しくない</span><span class="sxs-lookup"><span data-stu-id="e9e14-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9e14-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="e9e14-135">See also</span></span>

- [<span data-ttu-id="e9e14-136">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="e9e14-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="e9e14-137">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="e9e14-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="e9e14-138">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="e9e14-138">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

