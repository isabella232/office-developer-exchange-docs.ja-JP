---
title: GetMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTips
api_type:
- schema
ms.assetid: 4a24ff79-f1ae-43a1-9ac2-49baf3eaa173
description: GetMailTips ヒント要素は、取得するメールヒントの受信者と種類を表します。
ms.openlocfilehash: 8ff71ed5d52f713e11188b07c8c93aeee7dfa44d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458636"
---
# <a name="getmailtips"></a><span data-ttu-id="0107c-103">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="0107c-103">GetMailTips</span></span>

<span data-ttu-id="0107c-104">**Getmailtips**ヒント要素は、取得するメールヒントの受信者と種類を表します。</span><span class="sxs-lookup"><span data-stu-id="0107c-104">The **GetMailTips** element represents the recipients and types of mail tips to retrieve.</span></span> 
  
```XML
<GetMailTips>
   <SendingAs/>
   <Recipients/>
   <MailTipsRequested/>
</GetMailTips>
```

 <span data-ttu-id="0107c-105">**Getmailヒント Stype**</span><span class="sxs-lookup"><span data-stu-id="0107c-105">**GetMailTipsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0107c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0107c-106">Attributes and elements</span></span>

<span data-ttu-id="0107c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0107c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0107c-108">属性</span><span class="sxs-lookup"><span data-stu-id="0107c-108">Attributes</span></span>

<span data-ttu-id="0107c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0107c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0107c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0107c-110">Child elements</span></span>

|<span data-ttu-id="0107c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="0107c-111">**Element**</span></span>|<span data-ttu-id="0107c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0107c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0107c-113">SendingAs</span><span class="sxs-lookup"><span data-stu-id="0107c-113">SendingAs</span></span>](sendingas.md) <br/> |<span data-ttu-id="0107c-114">ユーザーが送信しようとしている電子メールアドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0107c-114">Contains an e-mail address that a user is trying to send as.</span></span>  <br/> |
|[<span data-ttu-id="0107c-115">受信者 (Arrayof受信者 Stype)</span><span class="sxs-lookup"><span data-stu-id="0107c-115">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md) <br/> |<span data-ttu-id="0107c-116">メールのヒントを確認する受信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0107c-116">Contains a list of recipients to check for mail tips.</span></span>  <br/> |
|[<span data-ttu-id="0107c-117">Mailヒント要求</span><span class="sxs-lookup"><span data-stu-id="0107c-117">MailTipsRequested</span></span>](mailtipsrequested.md) <br/> |<span data-ttu-id="0107c-118">サービスから要求されたメールヒントの種類が含まれます。</span><span class="sxs-lookup"><span data-stu-id="0107c-118">Contains the types of mail tips requested from the service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0107c-119">親要素</span><span class="sxs-lookup"><span data-stu-id="0107c-119">Parent elements</span></span>

<span data-ttu-id="0107c-120">なし。</span><span class="sxs-lookup"><span data-stu-id="0107c-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="0107c-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0107c-121">Text value</span></span>

<span data-ttu-id="0107c-122">なし。</span><span class="sxs-lookup"><span data-stu-id="0107c-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0107c-123">注釈</span><span class="sxs-lookup"><span data-stu-id="0107c-123">Remarks</span></span>

<span data-ttu-id="0107c-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0107c-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0107c-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0107c-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0107c-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="0107c-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0107c-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0107c-127">Schema Name</span></span>  <br/> |<span data-ttu-id="0107c-128">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0107c-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0107c-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0107c-129">Validation File</span></span>  <br/> |<span data-ttu-id="0107c-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0107c-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0107c-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0107c-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="0107c-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="0107c-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0107c-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="0107c-133">See also</span></span>



- [<span data-ttu-id="0107c-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0107c-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

