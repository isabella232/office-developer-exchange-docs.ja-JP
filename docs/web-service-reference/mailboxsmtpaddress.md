---
title: MailboxSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxSmtpAddress
api_type:
- schema
ms.assetid: de7c9035-ebbc-4473-ac14-3b22ce62768c
description: MailboxSmtpAddress 要素を取得または更新が受信トレイのルールは、ユーザーの SMTP アドレスを表しますか、パスワードの有効期限の日付が取得します。
ms.openlocfilehash: 60b2c018f2a05e9630e92e28de1054a421b41e52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832303"
---
# <a name="mailboxsmtpaddress"></a><span data-ttu-id="e085c-103">MailboxSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="e085c-103">MailboxSmtpAddress</span></span>

<span data-ttu-id="e085c-104">**MailboxSmtpAddress**要素を取得または更新が受信トレイのルールは、ユーザーの SMTP アドレスを表しますか、パスワードの有効期限の日付が取得します。</span><span class="sxs-lookup"><span data-stu-id="e085c-104">The **MailboxSmtpAddress** element represents the SMTP address of the user whose Inbox rules are to be retrieved or updated; or whose password expiration date is to be retrieved.</span></span> 
  
```XML
<MailboxSmtpAddress/>
```

<span data-ttu-id="e085c-105">**string**</span><span class="sxs-lookup"><span data-stu-id="e085c-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e085c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e085c-106">Attributes and elements</span></span>

<span data-ttu-id="e085c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e085c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e085c-108">属性</span><span class="sxs-lookup"><span data-stu-id="e085c-108">Attributes</span></span>

<span data-ttu-id="e085c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e085c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e085c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e085c-110">Child elements</span></span>

<span data-ttu-id="e085c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e085c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e085c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e085c-112">Parent elements</span></span>

|<span data-ttu-id="e085c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e085c-113">**Element**</span></span>|<span data-ttu-id="e085c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e085c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e085c-115">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="e085c-115">GetInboxRules</span></span>](getinboxrules.md) <br/> |<span data-ttu-id="e085c-116">サーバー ストア内のメールボックスの受信トレイ ルールを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="e085c-116">Defines a request to get the Inbox rules on a mailbox in the server store.</span></span>  <br/> |
|[<span data-ttu-id="e085c-117">GetPasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="e085c-117">GetPasswordExpirationDate</span></span>](getpasswordexpirationdate.md) <br/> |<span data-ttu-id="e085c-118">電子メール アカウントのパスワードの有効期限の日付を取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="e085c-118">Defines a request to get the password expiration date of an email account.</span></span>  <br/> |
|[<span data-ttu-id="e085c-119">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="e085c-119">UpdateInboxRules</span></span>](updateinboxrules.md) <br/> |<span data-ttu-id="e085c-120">サーバー ストア内のメールボックスの受信トレイ ルールを更新する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="e085c-120">Defines a request to update the Inbox rules in a mailbox in the server store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e085c-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e085c-121">Text value</span></span>

<span data-ttu-id="e085c-122">なし。</span><span class="sxs-lookup"><span data-stu-id="e085c-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e085c-123">備考</span><span class="sxs-lookup"><span data-stu-id="e085c-123">Remarks</span></span>

<span data-ttu-id="e085c-124">**MailboxSmtpAddress**要素は、省略可能な要素です。</span><span class="sxs-lookup"><span data-stu-id="e085c-124">The **MailboxSmtpAddress** element is an optional element.</span></span> <span data-ttu-id="e085c-125">**MailboxSmtpAddress**要素を省略すると、ログオンしたユーザーのアドレスが使用されます。</span><span class="sxs-lookup"><span data-stu-id="e085c-125">If the **MailboxSmtpAddress** element is omitted, the address of the logged on user is used.</span></span> 
  
<span data-ttu-id="e085c-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e085c-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e085c-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="e085c-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e085c-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="e085c-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e085c-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e085c-129">Schema Name</span></span>  <br/> |<span data-ttu-id="e085c-130">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e085c-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="e085c-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e085c-131">Validation File</span></span>  <br/> |<span data-ttu-id="e085c-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e085c-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e085c-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e085c-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="e085c-134">True</span><span class="sxs-lookup"><span data-stu-id="e085c-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e085c-135">関連項目</span><span class="sxs-lookup"><span data-stu-id="e085c-135">See also</span></span>

- [<span data-ttu-id="e085c-136">GetInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="e085c-136">GetInboxRules operation</span></span>](getinboxrules-operation.md)
- [<span data-ttu-id="e085c-137">GetPasswordExpirationDate 操作</span><span class="sxs-lookup"><span data-stu-id="e085c-137">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="e085c-138">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="e085c-138">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="e085c-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e085c-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

