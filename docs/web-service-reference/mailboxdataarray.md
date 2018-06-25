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
description: MailboxDataArray 要素には、利用可能時間情報のクエリを実行するメールボックスの一覧が含まれています。
ms.openlocfilehash: b76e71ee9127dc2221e0065a27d3c781f8b5786a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832283"
---
# <a name="mailboxdataarray"></a><span data-ttu-id="35f52-103">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="35f52-103">MailboxDataArray</span></span>

<span data-ttu-id="35f52-104">**MailboxDataArray**要素には、利用可能時間情報のクエリを実行するメールボックスの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="35f52-104">The **MailboxDataArray** element contains a list of mailboxes to query for availability information.</span></span> 
  
- [<span data-ttu-id="35f52-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="35f52-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
- [<span data-ttu-id="35f52-106">MailboxDataArray</span><span class="sxs-lookup"><span data-stu-id="35f52-106">MailboxDataArray</span></span>](mailboxdataarray.md)
  
- [<span data-ttu-id="35f52-107">MailboxData</span><span class="sxs-lookup"><span data-stu-id="35f52-107">MailboxData</span></span>](mailboxdata.md)
  
```xml
<MailboxDataArray>
   <MailboxData>...</MailboxData>
</MailboxDataArray>
```

<span data-ttu-id="35f52-108">**ArrayOfMailboxData**</span><span class="sxs-lookup"><span data-stu-id="35f52-108">**ArrayOfMailboxData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="35f52-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="35f52-109">Attributes and elements</span></span>

<span data-ttu-id="35f52-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="35f52-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="35f52-111">属性</span><span class="sxs-lookup"><span data-stu-id="35f52-111">Attributes</span></span>

<span data-ttu-id="35f52-112">なし。</span><span class="sxs-lookup"><span data-stu-id="35f52-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="35f52-113">子要素</span><span class="sxs-lookup"><span data-stu-id="35f52-113">Child elements</span></span>

|<span data-ttu-id="35f52-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="35f52-114">**Element**</span></span>|<span data-ttu-id="35f52-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="35f52-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35f52-116">MailboxData</span><span class="sxs-lookup"><span data-stu-id="35f52-116">MailboxData</span></span>](mailboxdata.md) <br/> |<span data-ttu-id="35f52-117">個々 のメールボックス ユーザーのメールボックスのユーザーに返されるデータの種類のオプションを表します。</span><span class="sxs-lookup"><span data-stu-id="35f52-117">Represents an individual mailbox user and options for the type of data to be returned about the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="35f52-118">親要素</span><span class="sxs-lookup"><span data-stu-id="35f52-118">Parent elements</span></span>

|<span data-ttu-id="35f52-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="35f52-119">**Element**</span></span>|<span data-ttu-id="35f52-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="35f52-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="35f52-121">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="35f52-121">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="35f52-122">ユーザーの利用可能時間情報を取得するための引数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="35f52-122">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="35f52-123">これは、ルート要素です。</span><span class="sxs-lookup"><span data-stu-id="35f52-123">This is a root element.</span></span>  <br/> <span data-ttu-id="35f52-124">以下は、この要素の XPath です。</span><span class="sxs-lookup"><span data-stu-id="35f52-124">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="35f52-125">備考</span><span class="sxs-lookup"><span data-stu-id="35f52-125">Remarks</span></span>

<span data-ttu-id="35f52-126">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft® Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="35f52-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="35f52-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="35f52-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="35f52-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="35f52-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="35f52-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="35f52-129">Schema Name</span></span>  <br/> |<span data-ttu-id="35f52-130">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="35f52-130">Messages schema</span></span>  <br/> |
|<span data-ttu-id="35f52-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="35f52-131">Validation File</span></span>  <br/> |<span data-ttu-id="35f52-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="35f52-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="35f52-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="35f52-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="35f52-134">False</span><span class="sxs-lookup"><span data-stu-id="35f52-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="35f52-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="35f52-135">See also</span></span>

- [<span data-ttu-id="35f52-136">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="35f52-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="35f52-137">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="35f52-137">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
- [<span data-ttu-id="35f52-138">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="35f52-138">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

